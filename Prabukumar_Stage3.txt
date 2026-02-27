# Stage 3: Student Grade Calculator

name = input("Enter student name: ")

mark1 = int(input("Enter mark for subject 1: "))
mark2 = int(input("Enter mark for subject 2: "))
mark3 = int(input("Enter mark for subject 3: "))

# Validate marks
if (0 <= mark1 <= 100) and (0 <= mark2 <= 100) and (0 <= mark3 <= 100):
    
    total = mark1 + mark2 + mark3
    percentage = (total / 300) * 100

    if percentage >= 75:
        grade = "A"
    elif percentage >= 60:
        grade = "B"
    elif percentage >= 40:
        grade = "C"
    else:
        grade = "F"

    print("Student Name:", name)
    print("Total:", total, "/300")
    print("Percentage:", percentage, "%")
    print("Grade:", grade)

else:
    print("Invalid marks!")