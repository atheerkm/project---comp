# project--camp

def get_grade(score)

score = round(score)

if   score<=100 and score>=0:

elif score>=90:
   print("A+")
elif score>=86:
   print("A")
elif score>=82:
   print("A-")
elif score>=78:
   print("B+")
 elif score>=74:
   print("B")
elif score>=70:
   print("B-")
elif score>=66:
   print("C+")
elif score>=62:
   print("C")
elif score>=58:
   print("C-")
elif score>=54:
   print("D")
elif score>=0:
   print("F")
else:
    print ("invalid score:")



def get_point(grade):

    if grade == "A+":
        return 4.00
    elif grade == "A":
        return 4.00
    elif grade == "A-":
        return 3.67
    elif grade == "B+":
        return 3.33
    elif grade == "B":
        return 3.00
    elif grade == "B-":
        return 2.67
    elif grade == "C+":
        return 2.33
    elif grade == "C":
        return 2.00
    elif grade == "C-":
        return 1.67
    elif grade == "D+":
        return 1.33
    elif grade == "D":
        return 1.00
    elif grade == "F":
        return 0


 def calculate(grade1=None, grade2=None, grade3=None):
    total_subject=0
    total_mark = 0

    if grade1 !=None:
        total_subject +=1
        grade1 = get_point(grade1)
        total_mark += grade1

    if grade2 != None:
       total_subject +=1
       grade2 = get_point(grade2)
       total_mark += grade2

   if grade3 != None:
      total_subject +=1
      grade3 = get_point(grade3)
      total_mark += grade3

   gpa = total_mark / total_subject
   print("your gpa is", gpa)

grade1 = input("Enter your grade:")
grade2 = input("Enter your grade:")
grade3 = input("Enter your grade:")

calculate_gpa(grade1,grade2,grade3)
