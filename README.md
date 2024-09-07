def fibonacci(n):
    fib_series = []
    a, b = 0, 1
    for _ in range(n):
        fib_series.append(a)
        a, b = b, a + b
    return fib_series

# Input: Number of terms
num_terms = int(input("Enter the number of terms: "))

# Generate and display the Fibonacci series
if num_terms <= 0:
    print("Please enter a positive integer.")
else:
    print("Fibonacci series:")
    print(fibonacci(num_terms))
