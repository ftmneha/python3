# python3
def is_prime(num):
    if num < 2:
        return False
    for i in range(2, int(num**0.5) + 1):
        if num % i == 0:
            return False
    return True

def print_even_primes_in_range(start, end):
    for num in range(start, end + 1):
        if num == 2 or (num % 2 == 0 and is_prime(num)):
            print(num, end=' ')
