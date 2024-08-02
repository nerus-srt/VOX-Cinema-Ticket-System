 # VOX Cinema Ticket System

## Project Overview

**Project Name**: VOX Cinema Ticket System  
**Objective**: To classify users into age categories for a cinema ticketing system.

## Project Requirements and Dependencies

- **Python**: Used to write the script.
- **No additional libraries required**.

## Steps

1. **User Input**:
   - Prompt the user to enter their name.
   - Prompt the user to enter their age.

2. **Age Category Classification**:
   - If the user is under 13 years old, classify them as a child.
   - If the user is 13 years old or older, classify them as a senior.

## Code

```python
# Programmer: Suren Raj Tuladhar
# Date: 13/07/2022
# Program: VOX Cinema Ticket System

def get_user_input():
    name = input("Enter your name: ")
    age = input("Enter your age: ")
    return name, age

def classify_age(age):
    try:
        age = int(age)
        if age < 13:
            print("You belong to the children category")
        else:
            print("You belong to the senior category")
            print("Thank you for using our ticketing system")
    except ValueError:
        print("Invalid input for age. Please enter a number.")

def main():
    name, age = get_user_input()
    classify_age(age)

if __name__ == "__main__":
    main()
