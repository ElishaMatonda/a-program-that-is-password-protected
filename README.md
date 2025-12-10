# a-program-that-is-password-protected

#python
#Pre-set password
correct_password ="12TUK??"
attempts = 0
max_attempts = 3

Login system
while attempts < max_attempts:
    password = input("Enter password: ")
    if password == correct_password:
        print("Login successful.\n")
        break
    else:
        attempts += 1
        print(f"Wrong password. Attempts left: {max_attempts - attempts}")
else:
    print("Too many failed attempts. Access denied.")
    exit()

Grading system
try:
    mark = float(input("Enter student's mark (0–100): "))
    if 80 <= mark <= 100:
        grade = 'A'
    elif 70 <= mark < 80:
        grade = 'B'
    elif 60 <= mark < 70:
        grade = 'C'
    elif 50 <= mark < 60:
        grade = 'D'
    elif 0 <= mark < 50:
        grade = 'F'
    else:
        grade = 'Invalid mark'
    
    print(f"Grade: {grade}")

except ValueError:
    print("Invalid input. Please enter a number.")
