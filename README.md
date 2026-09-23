# Python---Data---Science--Mini--Project-
Python for data science mini project 
# Student Performance Analysis
# Python for Data Science Mini Project

import statistics
students = ["Arun", "Bala", "Charan", "Divya", "Esha"]
marks = [78, 65, 89, 92, 56]
average = statistics.mean(marks)
highest = max(marks)
lowest = min(marks)
print("=" * 40)
print("       STUDENT PERFORMANCE ANALYSIS")
print("=" * 40)
print("\nStudent Marks:")
for i in range(len(students)):
    print(f"{students[i]:10} : {marks[i]}")
print("\n" + "-" * 40)
print(f"Average Mark : {average:.2f}")
print(f"Highest Mark : {highest}")
print(f"Lowest Mark  : {lowest}")
print("-" * 40)
topper_index = marks.index(highest)
print(f"Topper       : {students[topper_index]}")
print("\nPerformance Status:")
for i in range(len(students)):
    if marks[i] >= 80:
        status = "Excellent"
    elif marks[i] >= 60:
        status = "Good"
    else:
        status = "Needs Improvement"
    print(f"{students[i]:10} : {status}")
print("\nAnalysis Completed Successfully!")
