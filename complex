class Complex:
    def __init__(self, x, y):
        self.x = x  # Real part
        self.y = y  # Imaginary part

    def __add__(self, other):
        # Return a new Complex object
        return Complex(self.x + other.x, self.y + other.y)

    def __sub__(self, other):
        # Return a new Complex object
        return Complex(self.x - other.x, self.y - other.y)

    def __str__(self):
        # Nicely format the complex number
        if self.y >= 0:
            return f"{self.x} + {self.y}j"
        else:
            return f"{self.x} - {abs(self.y)}j"


# Input for first complex number
x1 = int(input("Enter real part of first number: "))
y1 = int(input("Enter imaginary part of first number: "))
c1 = Complex(x1, y1)

# Input for second complex number
x2 = int(input("Enter real part of second number: "))
y2 = int(input("Enter imaginary part of second number: "))
c2 = Complex(x2, y2)

# Perform operations
print("ADDITION OF COMPLEX:", c1 + c2)
print("SUBTRACTION OF COMPLEX:", c1 - c2)
