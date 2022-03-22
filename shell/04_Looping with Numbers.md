# Looping with Numbers

## Problem

Use a for loop to display the natural numbers from `1` to `50`.

**Input Format**

There is no input

**Output Format**

```
1
2
3
4
5
.
.
.
.
.
50
```

## Codes
```bash
for i in $(seq 1 50); do echo "${i}"; done
```