# -Semester-work
file = open("c:\\Users\\ASUS TUF\\Desktop\\kr\\results.txt", "r")
lines = file.readlines()
file.close()

AAA = input("Введіть температуру: ")

AAA = float(AAA)

times = []

for line in lines:
    time, XXX = line.split()

    XXX = float(XXX)

    if XXX > AAA:
        times.append(time)

print("Час, при якому температура перевищує температуру - ", AAA , "градусів: ", times)
