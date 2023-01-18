## Description

<div><p>You invited $n$ guests to dinner! You plan to arrange one or more circles of chairs. Each chair is going to be either occupied by one guest, or be empty. You can make any number of circles. </p><p>Your guests happen to be a little bit shy, so the $i$-th guest wants to have a least $l_i$ free chairs to the left of his chair, and at least $r_i$ free chairs to the right. The "left" and "right" directions are chosen assuming all guests are going to be seated towards the center of the circle. Note that when a guest is the only one in his circle, the $l_i$ chairs to his left and $r_i$ chairs to his right may overlap.</p><p>What is smallest total number of chairs you have to use?</p></div><div class="input-specification"><p>First line contains one integer $n$ &nbsp;— number of guests, ($1 \leqslant n \leqslant 10^5$). </p><p>Next $n$ lines contain $n$ pairs of space-separated integers $l_i$ and $r_i$ ($0 \leqslant l_i, r_i \leqslant 10^9$).</p></div><div class="output-specification"><p>Output a single integer&nbsp;— the smallest number of chairs you have to use.</p></div>

## Input

<p>First line contains one integer $n$ &nbsp;— number of guests, ($1 \leqslant n \leqslant 10^5$). </p><p>Next $n$ lines contain $n$ pairs of space-separated integers $l_i$ and $r_i$ ($0 \leqslant l_i, r_i \leqslant 10^9$).</p>

## Output

<p>Output a single integer&nbsp;— the smallest number of chairs you have to use.</p>





```input1
3
1 1
1 1
1 1

```




```input2
4
1 2
2 1
3 5
5 3

```




```input3
1
5 6

```




```output1
6

```




```output2
15

```




```output3
7

```



## Note

<p>In the second sample the only optimal answer is to use two circles: a circle with $5$ chairs accomodating guests $1$ and $2$, and another one with $10$ chairs accomodationg guests $3$ and $4$.</p><p>In the third sample, you have only one circle with one person. The guest should have at least five free chairs to his left, and at least six free chairs to his right to the next person, which is in this case the guest herself. So, overall number of chairs should be at least 6+1=7.</p>
