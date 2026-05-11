class Vector:

    def __init__(self, values):
        self.values = values

    # Addition
    def __add__(self, other):

        result = []

        for i in range(len(self.values)):
            result.append(self.values[i] + other.values[i])

        return result

    # Subtraction
    def __sub__(self, other):

        result = []

        for i in range(len(self.values)):
            result.append(self.values[i] - other.values[i])

        return result

    # Scalar Multiplication
    def __mul__(self, scalar):

        result = []

        for i in self.values:
            result.append(i * scalar)

        return result

    # Equality
    def __eq__(self, other):

        return self.values == other.values

    # Dot Product
    def dot(self, other):

        total = 0

        for i in range(len(self.values)):
            total += self.values[i] * other.values[i]

        return total

    # Cross Product
    def cross(self, other):

        a = self.values
        b = other.values

        return [
            a[1]*b[2] - a[2]*b[1],
            a[2]*b[0] - a[0]*b[2],
            a[0]*b[1] - a[1]*b[0]
        ]


# Input
v1 = list(map(int, input("Enter first vector: ").split()))

v2 = list(map(int, input("Enter second vector: ").split()))

s = int(input("Enter scalar value: "))

# Creating objects
obj1 = Vector(v1)
obj2 = Vector(v2)

# Operations
print("Addition =", obj1 + obj2)

print("Subtraction =", obj1 - obj2)

print("Scalar Multiplication =", obj1 * s)

print("Equal =", obj1 == obj2)

print("Dot Product =", obj1.dot(obj2))

# Cross Product Condition
if len(v1) == 3 and len(v2) == 3:

    print("Cross Product =", obj1.cross(obj2))

else:

    print("Cross Product possible only for 3 values")
