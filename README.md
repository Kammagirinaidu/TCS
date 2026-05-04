# TCS
# Sum of Digits
n = int(input())
sum = 0
while n > 0:
    sum += n % 10
    n //= 10
print(sum)
# Check Prime Number
n = int(input())
if n < 2:
    print("Not Prime")
else:
    for i in range(2, int(n**0.5) + 1):
        if n % i == 0:
            print("Not Prime")
            break
    else:
        print("Prime")
# Reverse a Number
n = int(input())
rev = 0
while n > 0:
    rev = rev * 10 + (n % 10)
    n //= 10
print(rev)
# Fibonacci Series
n = int(input())
a, b = 0, 1
for i in range(n):
    print(a, end=" ")
    a, b = b, a + b
# Armstrong Number
n = int(input())
temp = n
power = len(str(n))
sum = 0

while temp > 0:
    digit = temp % 10
    sum += digit ** power
    temp //= 10

print("Yes" if sum == n else "No")
# Palindrome Number
n = input()
print("Yes" if n == n[::-1] else "No")
# Factorial of a number
n = int(input())
fact = 1
for i in range(1, n + 1):
    fact *= i
print(fact)
# Count Vowels in String
s = input().lower()
count = 0
for ch in s:
    if ch in "aeiou":
        count += 1
print(count)
# Second Largest Element
arr = list(map(int, input().split()))
arr = list(set(arr))
arr.sort()
print(arr[-2])
# Remove Duplicates from List
arr = list(map(int, input().split()))
result = list(set(arr))
print(result)
