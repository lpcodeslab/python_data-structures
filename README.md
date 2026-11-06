# python_data-structures
Python assignment demonstrating the use of lists, dictionaries, sets, and conditional statements with practical examples.
# 1. List Creation

age_list = [24, 25, 26, 27, 28]
name_list = ["Arun", "Priya", "Kavi", "Ravi", "Meena"]

print("Age List:", age_list)
print("Name List:", name_list)


# 2. List Operations / Modifications

# a. Append Yazhini
name_list.append("Yazhini")
print("After Append:", name_list)

# b. Insert 30 at index 2
age_list.insert(2, 30)
print("After Insert:", age_list)

# c. Remove Yazhini
name_list.remove("Yazhini")
print("After Remove:", name_list)

# d. Pop the last element
age_list.pop()
print("After Pop:", age_list)

# e. Extend age_list
age_list.extend([29, 30, 26])
print("After Extend:", age_list)

# f. Sort in descending order
age_list.sort(reverse=True)
print("Descending Order:", age_list)

# g. Find maximum, minimum and sum
print("Maximum Age:", max(age_list))
print("Minimum Age:", min(age_list))
print("Sum of Ages:", sum(age_list))


# 3. Accessing List Elements

# a. First element
print("First Name:", name_list[0])

# b. Last element
print("Last Name:", name_list[-1])

# c. Elements from index 2 to 4
print("Index 2 to 4:", name_list[2:5])

# d. Reverse order
print("Reverse Order:", name_list[::-1])

# 4. Dictionary

# a. Create a dictionary

student_marks = {
    "Arun": 75,
    "Priya": 90,
    "Kavi": 85,
    "Ravi": 70,
    "Meena": 95
}

print("Student Marks:", student_marks)

# b. Access and print a student's mark
print("Priya's Mark:", student_marks["Priya"])

# c. Add a new student
student_marks["Janani"] = 80
print("After Adding Janani:", student_marks)

# d. Update an older student's mark to 82
student_marks["Arun"] = 82
print("After Updating Mark:", student_marks)

# e. Print all keys
print("Student Names:", student_marks.keys())

# Print all values
print("Student Marks:", student_marks.values())

# Print all key-value pairs
print("Student Details:", student_marks.items())

# 5. Sets

# a. Create a set

my_set = {'a', 'e', 'i', 'o', 'u', 'a', 'a', 'i'}

print("My Set:", my_set)

# Explanation:
# A set does not allow duplicate values.
# Therefore, repeated elements are removed automatically.
# The order of elements is not guaranteed.


# b. Attempt to change a set element

try:
    my_set[4] = 's'
except TypeError as e:
    print("Error:", e)

# Explanation:
# Sets are unindexed and do not support item assignment.
# Therefore, individual elements cannot be changed.


# c. Create two sets

set1 = {1, 3, 5, 7, 9}
set2 = {2, 3, 5, 8, 10}

# d. Union and Intersection

print("Union:", set1.union(set2))

print("Intersection:", set1.intersection(set2)) 

# 6. Operators & Conditional Statements :

# Performance Category Program

score = int(input("Enter your score (0 to 10): "))

if score < 0 or score > 10:
    print("Invalid score! Please enter a score between 0 and 10.")

elif score > 7:
    print("Above Average: Excellent performance! Keep it up.")

elif score >= 4:
    print("Average: Good effort! Keep practicing, there's room for improvement.")

else:
    print("Below Average: Need to improve your performance. Consistent practice will lead to better results.")
