# Day-6-Prime-Number-Checker
Day 6/100 - Python Program to Check prime number

# Prime Number Checker
A program to determine whether a given integer is a prime number using a loop and basic divisibility checks.

## 📝 Description

This program evaluates a user-inputted number to check if it is a prime number. A prime number is a whole number greater than 1 whose only divisors are 1 and itself. The script utilizes a `for` loop to divide the number by all integers from 2 up to the number itself minus one. If any of these divisions result in a remainder of 0 (`num % i == 0`), the number is not prime. It also elegantly uses Python's `for...else` construct to confirm a prime number if the loop completes without ever triggering a `break`.

---

## 🎯 Problem Statement

### Input:

* A single integer value.

### Output:

* A formatted string stating: "[num] is a prime number." or "[num] is not a prime number."

### Rules:

1. The program must accept an integer input from the user.
2. If the number is strictly greater than 1, it must be checked for primality.
3. The program iterates from 2 up to `num - 1`. If the number is evenly divisible by any of these values, it is **not prime**.
4. If the loop finishes without finding any divisors, the number **is prime**.
5. If the initial number is 1, 0, or negative, it immediately falls to the `else` block and is declared **not prime**.

---

## 💡 Examples

### Example 1

**Input:**

```
7

```

**Output:**

```
7 is a prime number.

```

**Explanation:** The number 7 is greater than 1. The loop checks if 7 is divisible by 2, 3, 4, 5, or 6. Since none of these yield a remainder of 0, the `else` block executes, declaring it prime.

### Example 2

**Input:**

```
10

```

**Output:**

```
10 is not a prime number.

```

**Explanation:** The loop checks divisors starting from 2. Since `10 % 2 == 0` is true, the program prints that it is not prime and breaks out of the loop immediately.

### Example 3 (Edge Case: 1)

**Input:**

```
1

```

**Output:**

```
1 is not a prime number.

```

**Explanation:** The initial `if num > 1` condition is false, so the program skips the loop and directly prints that 1 is not prime.

### Example 4 (Negative Number)

**Input:**

```
-5

```

**Output:**

```
-5 is not a prime number.

```

**Explanation:** Similar to Example 3, negative numbers fail the `num > 1` check and are immediately classified as not prime.

---

## 🚀 How to Use

1. **Clone this repository** (or save the script)
```bash
git clone https://github.com/adiaryaz/Day6-Prime-Number-Checker.git
cd prime-number-checker

```


2. **Run the program**:
```bash
python main.py

```


Enter an integer when prompted by "Enter a number: " to see if it is a prime number.
