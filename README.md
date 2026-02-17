# repo2
def fibonacci_series(n):
    a, b = 0, 1
    count = 0
    
    if n <= 0:
        print("Please enter a positive integer")
    elif n == 1:
        print(a)
    else:
        print("Fibonacci series:")
        while count < n:
            print(a, end=" ")
            nth = a + b
            # Update values
            a = b
            b = nth
            count += 1

# Example usage
n = int(input("How many terms? "))
fibonacci_series(n)
