class Polynomial:

    def __init__(self, coeff):
        self.coeff = coeff

    # Operator overloading using *
    def __mul__(self, other):

        first_poly = self.coeff
        second_poly = other.coeff

        result = [0] * (len(first_poly) + len(second_poly) - 1)

        for i in range(len(first_poly)):
            for j in range(len(second_poly)):
                result[i + j] += first_poly[i] * second_poly[j]

        return result


# Getting input from user
p1 = list(map(int, input("ENTER FIRST POLYNOMIAL COEFFICIENTS: ").split()))

p2 = list(map(int, input("ENTER SECOND POLYNOMIAL COEFFICIENTS: ").split()))

# Creating objects
obj1 = Polynomial(p1)
obj2 = Polynomial(p2)

# Multiplying polynomials
print("Result =", obj1 * obj2)
