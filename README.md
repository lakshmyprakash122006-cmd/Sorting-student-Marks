# Sorting-student-Marks
Data structure practical program 
# Bubble Sort to sort student marks

students = [
    {"name": "Ravi", "marks": 85},
    {"name": "Anu", "marks": 92},
    {"name": "Kiran", "marks": 78},
    {"name": "Priya", "marks": 90}
]

# Sorting marks using Bubble Sort
n = len(students)
for i in range(n):
    for j in range(0, n - i - 1):
        if students[j]["marks"] > students[j + 1]["marks"]:
            students[j], students[j + 1] = students[j + 1], students[j]

print("Students sorted by marks (ascending):")
for student in students:
    print(f"{student['name']}: {student['marks']}")

  output:
  Students sorted by marks (ascending):
Kiran: 78
Ravi: 85
Priya: 90
Anu: 92
