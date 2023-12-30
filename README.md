# endoflineLoop


def endofline():
    fileName = input("What is the name of a file? ")
    infile = open(fileName, "r")
    total = 0
    count = 0
    line = infile.readline()
    while line != "":
        total += float(line)
        count += 1
        line = infile.readline()
    print("Average of the numbers is", total / count)

endofline()
