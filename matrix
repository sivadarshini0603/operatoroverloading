class Matrix:

    def __init__(self, matrix):
        self.matrix = matrix

    # Addition
    def __add__(self, other):

        result = []

        for i in range(len(self.matrix)):
            row = []

            for j in range(len(self.matrix[0])):
                row.append(self.matrix[i][j] + other.matrix[i][j])

            result.append(row)

        return result

    # Subtraction
    def __sub__(self, other):

        result = []

        for i in range(len(self.matrix)):
            row = []

            for j in range(len(self.matrix[0])):
                row.append(self.matrix[i][j] - other.matrix[i][j])

            result.append(row)

        return result

    # Multiplication
    def __mul__(self, other):

        result = [[0 for j in range(len(other.matrix[0]))]
                  for i in range(len(self.matrix))]

        for i in range(len(self.matrix)):
            for j in range(len(other.matrix[0])):
                for k in range(len(other.matrix)):
                    result[i][j] += self.matrix[i][k] * other.matrix[k][j]

        return result


# Input for first matrix
r1 = int(input("Enter rows of first matrix: "))
c1 = int(input("Enter columns of first matrix: "))

m1 = []

print("Enter first matrix elements:")

for i in range(r1):
    row = list(map(int, input().split()))
    m1.append(row)


# Input for second matrix
r2 = int(input("Enter rows of second matrix: "))
c2 = int(input("Enter columns of second matrix: "))

m2 = []

print("Enter second matrix elements:")

for i in range(r2):
    row = list(map(int, input().split()))
    m2.append(row)


# Creating objects
obj1 = Matrix(m1)
obj2 = Matrix(m2)


# Addition and Subtraction
if r1 == r2 and c1 == c2:

    print("Addition =", obj1 + obj2)
    print("Subtraction =", obj1 - obj2)

else:
    print("Addition and Subtraction not possible")


# Multiplication
if c1 == r2:

    print("Multiplication =", obj1 * obj2)

else:
    print("Multiplication not possible")
