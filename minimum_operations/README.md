# Minimum Operations

This project contains a method that calculates the fewest number of operations needed to result in exactly `n` H characters in a text file, starting with a single H character.

## Operations Available

- **Copy All**: Copies all characters currently in the file
- **Paste**: Pastes the copied characters

## Usage

```python
minOperations = __import__('0-minoperations').minOperations

n = 9
print(minOperations(n))  # Output: 6
```

## Algorithm

The solution uses prime factorization. For each prime factor `p` of `n`, we need `p` operations (1 Copy All + (p-1) Paste operations). The total minimum operations is the sum of all prime factors.

## Files

- `0-minoperations.py`: Contains the `minOperations(n)` function
