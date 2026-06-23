# Debugging Sequential String Matching

## Problem Statement
The given brute-force string matching algorithm fails to detect some valid pattern occurrences because of an error in the loop condition.

## Given Code

```python
def string_match(text, pattern):
    n, m = len(text), len(pattern)

    for i in range(n-m):     # ERROR
        j = 0

        while j < m and text[i+j] == pattern[j]:
            j += 1

        if j == m:
            return i

    return -1
```

## Error Identification
The loop

```python
for i in range(n-m)
```

skips the last possible alignment.

The correct statement is:

```python
for i in range(n-m+1)
```

## Effect of the Error
Some valid occurrences of the pattern are not checked.

Example:

```python
text = "ABCDE"
pattern = "DE"
```

The pattern starts at index 3, but the algorithm never checks that position.

## Corrected Program

```python
def string_match(text, pattern):
    n, m = len(text), len(pattern)

    for i in range(n - m + 1):
        j = 0

        while j < m and text[i + j] == pattern[j]:
            j += 1

        if j == m:
            return i

    return -1


text = "ABCDE"
pattern = "DE"

print("Pattern found at index:", string_match(text, pattern))
```

## Output

```text
Pattern found at index: 3
```

## Worst-Case Time Complexity

```text
O(nm)
```

where:

- n = length of text
- m = length of pattern

## Space Complexity

```text
O(1)
```

## Conclusion
After correcting the loop condition, the algorithm checks every possible alignment and correctly finds all valid pattern occurrences.