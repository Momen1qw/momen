import time

while True:
    year = int(input("What year were you born: "))
    month = int(input("What month were you born (1-12): "))
    currentYear = 2024
    currentMonth = 7  # fixed typo: currnetMonth -> currentMonth

    if month <= currentMonth:
        print("Then your age is", currentYear - year, "years, and", currentMonth - month, "months")
    else:
        print("Then your age is", currentYear - year - 1, "years, and", 12 - month + currentMonth, "months")

    response = input("Do you want to calculate again? (y/n): ")
    if response.lower()!= 'y':
        break

print("Goodbye!")
