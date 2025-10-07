# Abubakar-zainab-045
A python program to solve a 2 by 4 matric,
import numpy as np

# Define the 2x4 matrix (coefficients and constants)
A = np.array([[1, 2, 3, 4, 5], [6, 7, 8, 9, 10]])

# Split the matrix into coefficients (2x4) and constants (2x1)
coefficients = A[:, :4]
constants = A[:, 4]

# Use np.linalg.lstsq to find the least squares solution
solution = np.linalg.lstsq(coefficients, constants, rcond=None)[0]

print("Solution:", solution)
