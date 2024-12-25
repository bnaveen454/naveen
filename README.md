## About me
My name is Banoth Naveen


##checking for strong password

def is_strong_password(password):
      
   if len(password)<8:
        return false
   if not any(char.isdigit() for char in password):
       return False
   if not any(char.lower() for char in password):
       return False
   if not any(char.upper() for char in password):
       return False
   if not any(char in '!@#$%^&*()_' for char in password):
        return False
   return True

print(is_strong_password("@weaHNA"))
print(is_strong_password("kRiA@092"))
