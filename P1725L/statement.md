## Description

<div><p>Pak Chanek is participating in a lemper cooking competition. In the competition, Pak Chanek has to cook lempers with $N$ stoves that are arranged sequentially from stove $1$ to stove $N$. Initially, stove $i$ has a temperature of $A_i$ degrees. A stove can have a negative temperature.</p><p>Pak Chanek realises that, in order for his lempers to be cooked, he needs to keep the temperature of each stove at a non-negative value. To make it happen, Pak Chanek can do zero or more operations. In one operation, Pak Chanek chooses one stove $i$ with $2 \leq i \leq N-1$, then:</p><ol> <li> changes the temperature of stove $i-1$ into $A_{i-1} := A_{i-1} + A_{i}$, </li><li> changes the temperature of stove $i+1$ into $A_{i+1} := A_{i+1} + A_{i}$, and </li><li> changes the temperature of stove $i$ into $A_i := -A_i$. </li></ol><p>Pak Chanek wants to know the minimum number of operations he needs to do such that the temperatures of all stoves are at non-negative values. Help Pak Chanek by telling him the minimum number of operations needed or by reporting if it is not possible to do.</p></div><div class="input-specification"><p>The first line contains a single integer $N$ ($1 \le N \le 10^5$) — the number of stoves.</p><p>The second line contains $N$ integers $A_1, A_2, \ldots, A_N$ ($-10^9 \leq A_i \leq 10^9$) — the initial temperatures of the stoves.</p></div><div class="output-specification"><p>Output an integer representing the minimum number of operations needed to make the temperatures of all stoves at non-negative values or output $-1$ if it is not possible.</p></div>

## Input

<p>The first line contains a single integer $N$ ($1 \le N \le 10^5$) — the number of stoves.</p><p>The second line contains $N$ integers $A_1, A_2, \ldots, A_N$ ($-10^9 \leq A_i \leq 10^9$) — the initial temperatures of the stoves.</p>

## Output

<p>Output an integer representing the minimum number of operations needed to make the temperatures of all stoves at non-negative values or output $-1$ if it is not possible.</p>





```input1
7
2 -1 -1 5 2 -2 9
```




```input2
5
-1 -2 -3 -4 -5
```




```output1
4
```




```output2
-1
```



## Note

<p>For the first example, a sequence of operations that can be done is as follows: </p><ul> <li> Pak Chanek does an operation to stove $3$, $A = [2, -2, 1, 4, 2, -2, 9]$. </li><li> Pak Chanek does an operation to stove $2$, $A = [0, 2, -1, 4, 2, -2, 9]$. </li><li> Pak Chanek does an operation to stove $3$, $A = [0, 1, 1, 3, 2, -2, 9]$. </li><li> Pak Chanek does an operation to stove $6$, $A = [0, 1, 1, 3, 0, 2, 7]$. </li></ul><p>There is no other sequence of operations such that the number of operations needed is fewer than $4$.</p>
