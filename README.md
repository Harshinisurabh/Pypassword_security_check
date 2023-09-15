# Pypassword_security_check
The password strength checker is a simple yet an very essential tool that is designed to access the strength of the passwords  and help the users to create more online credentials secure online  
# Check if the password length is at least 8 characters
if len(password) >= 8:
    strength += 1

# Check if the password contains both uppercase and lowercase letters
if re.search(r'[a-z]', password) and re.search(r'[A-Z]', password):
    strength += 1

# Check if the password contains at least one digit
if re.search(r'\d', password):
    strength += 1

# Check if the password contains at least one special character
if re.search(r'[!@#$%^&*()_+{}\[\]:;<>,.?~\\\-]', password):
    strength += 1

return strength
