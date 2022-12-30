# coding_troops_KOC11_Cipherschools
# Function to print the name of student who
# stood first after updation in rank
def nameRank(names, marks, updates, n):
    x=[]
    x=x+marks
    for i in range(0, n):
        marks[i] = marks[i] + updates[i]
    # Finding the highest marks
    print(marks)
    c = max(marks)
    z=marks.index(c)
    pm=x[z]
    x.sort(reverse=True)
    h=x.index(pm)
    print(": Name   : Marks : Current rank : Previous rank :")
    print(":", name[z], " " * (9 - len(name[z])), ":", marks[z], " " * (7 - len(marks)), ":", 1, " "*12, ":",h+1)


# Names of the students
name= ["harsh", "ayush", "yogesh"]

# Marks of the students
marks = [79,80,50]

# Updates that are to be done
updates = [20,-15,10]

# Number of students
n = len(marks)

nameRank(name, marks, updates, n)
