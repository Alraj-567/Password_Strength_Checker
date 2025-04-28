import re

def Check_Password_Strength(password):
    if len(password)<8:
        return "Weak Password of length less than 8 . Please Make it Strong"
    
    if not any(char.isdigit() for char in password):
        return "Your Password Lacks numbers . Add atleast one number "
    
    if not any(char.isupper() for char in password):
        return "Your password must contain an Upper Character"

    if not any(char.islower() for char in password):
        return "Your Password must contain lower character"

    if not re.search(r'[!@#%^&*(){}<>.?]',password):
        return "Your password must contain Special Characters"

    return "Your Password is Strong Enough"
def password_checker():
    print("Welcome to password strength checker !!")
    while True:
        password = input("Enter your password(type 'exit' to quit) : ")
        if password.lower() == 'exit':
            print("Thank You for Using Password Strength Checker")
            break
        result = Check_Password_Strength(password)
        print(result)

if __name__ == "__main__":
    password_checker()


