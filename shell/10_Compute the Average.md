# Compute the Average

## Problem
Given `N` integers, compute their average, rounded to three decimal places.

**Input Format**

The first line contains an integer, `N`.<br>
Each of the following `N` lines contains a single integer.

**Output Format**

Display the average of the `N` integers, rounded off to three decimal places.

**Input Constraints**

1 ≦ `N` ≦ 500

-10000 ≦ `x` ≦ 10000 (`x` refers to elements of the list of integers for which the average is to be computed)

**Sample Input**

```
4
1
2
9
8
```

**Sample Output**

```
5.000
```

**Explanation**

The '4' in the first line indicates that there are four integers whose average is to be computed.

The average = (1 + 2 + 9 + 8)/4 = 20/4 = 5.000 (correct to three decimal places).

Please include the zeroes even if they are redundant (e.g. 0.000 instead of 0).

## Codes

```bash
read num
for ((i=0;i<${num};i++)); do
    read -p "" line
    lines+=("${line}")
#    total=$(echo "${total}+${lines[$i]}" | bc)
done

total=0
for ((i=0;i<${num};i++)); do
    total=$(expr ${total} + ${lines[$i]})
done

printf "%.3f" $(echo "scale=4; (${total})/${num}" | bc)
```