# Looping and Skipping

## Problem
Your task is to use for loops to display only odd natural numbers from `1` to `99`.

**Input Format**

There is no input.

**Constraints**

`-`

**Output Format**
```
1
3
5
.
.
.
.
.
99
```

**Sample Input**

`-`

**Sample Output**

```
1
3
5
.
.
.
.
.
99  
```

**Explanation**

`-`

## Codes

```bash
for ((i=1;i<100;i=i+2)); do
    echo ${i}
done
```