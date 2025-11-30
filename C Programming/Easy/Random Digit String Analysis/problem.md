# 🟢 Random Digit String Analysis

**Recommended Time:** 10 - 15 min

**Topics:** Strings, Control Structures (Loops), Random Numbers

## Task
Write a C program that performs the following steps:

1. Generate a random string of exactly 20 digits (characters `'0'` through `'9'`). Use C's random number generation facilities and seed the generator appropriately (e.g., with `time(NULL)`).
2. Display the generated sequence to the user.
3. Prompt the user to enter a single digit character to search for.
4. Count how many times the user's digit appears within the generated random string.
5. Output the final count in a clear sentence.

## Input / Output
- **Input:** The program generates a 20-digit string and reads one digit character from standard input.
- **Output:** A printed sentence showing how many times the chosen digit appears in the generated string.

## Requirements
- The generated string must be exactly 20 characters long and composed only of digits `'0'`–`'9'`.
- Properly seed the random number generator (for example with `srand((unsigned)time(NULL))`).
- Read the user's digit as a `char` and validate it is a digit (optional but recommended).
- Count occurrences by iterating the generated string once.
- Print the count in a clear sentence such as: `Digit 9 appears 3 times.`

## Examples

```text
Example 1:
Generated: 10395820495720394855
User input: 9
Output: Digit 9 appears 3 times.
```

```text
Example 2:
Generated: 22718366901235489762
User input: 2
Output: Digit 2 appears 5 times.
```

```text
Example 3:
Generated: 31415926535897932384
User input: 0
Output: Digit 0 appears 0 times.
```

---

**Note:** Because of the use of random, there is no `testing.c`. Based on the outputs, is it actually random?