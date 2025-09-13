# Minimum Operations

## Description
This project implements a solution to find the minimum number of operations needed to result in exactly n H characters in a text file, where the only allowed operations are "Copy All" and "Paste".

## Problem Statement
In a text file, there is a single character H. Your text editor can execute only two operations in this file: Copy All and Paste. Given a number n, write a method that calculates the fewest number of operations needed to result in exactly n H characters in the file.

## Algorithm
The solution uses prime factorization to determine the minimum operations:
- Each prime factor represents a copy-paste operation
- The sum of all prime factors gives the minimum number of operations
- If n is impossible to achieve (n ≤ 1), return 0

## Files
- `0-minoperations.py`: Contains the `minOperations` function
- `0-main.py`: Test file to verify the implementation

## Usage
```bash
python3 0-main.py
```

## Example
For n = 9:
- H → Copy All → Paste → HH → Paste → HHH → Copy All → Paste → HHHHHH → Paste → HHHHHHHHH
- Number of operations: 6

## Requirements
- Python 3.4.3
- Ubuntu 14.04 LTS
- All files must be executable
- Code follows PEP 8 style
