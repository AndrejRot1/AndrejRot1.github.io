Let's have some fun with prime numbers !

# Find if a number is prime or not

def prime(num = int):
    prime = False
    for index in range(1,num):
        if (num % index == 0) and (index != 1):
            return print(num,'Its not a prime')
    prime = True
    return print(num,'Its a prime num'),prime


# Lets find prime numbers in a range

def prime_range(a = int, b = int):
    for index in range(a,b + 1):
        prime(index)

# Split number into prime numbers

def split_into_primes(num = int):
    set_of_primes = []
    for index in range(2,num + 1):
        prime(index)
        if prime == True:
            set_of_primes.append(index)
    return set_of_primes
