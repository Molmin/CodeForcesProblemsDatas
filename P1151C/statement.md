## Description

<div><p>Nazar, a student of the scientific lyceum of the Kingdom of Kremland, is known for his outstanding mathematical abilities. Today a math teacher gave him a <span class="tex-font-style-tt">very difficult task</span>.</p><p>Consider two infinite sets of numbers. The first set consists of odd positive numbers ($1, 3, 5, 7, \ldots$), and the second set consists of even positive numbers ($2, 4, 6, 8, \ldots$). At the first stage, the teacher writes the first number on the endless blackboard from the first set, in the second stage&nbsp;— the first two numbers from the second set, on the third stage&nbsp;— the next four numbers from the first set, on the fourth&nbsp;— the next eight numbers from the second set and so on. In other words, at each stage, starting from the second, he writes out <span class="tex-font-style-bf">two times more</span> numbers than at the previous one, and also <span class="tex-font-style-bf">changes the set</span> from which these numbers are written out <span class="tex-font-style-bf">to another</span>. </p><p>The ten first written numbers: $1, 2, 4, 3, 5, 7, 9, 6, 8, 10$. Let's number the numbers written, starting <span class="tex-font-style-bf">with one</span>.</p><p>The task is to find the sum of numbers with numbers from $l$ to $r$ for given integers $l$ and $r$. The answer may be big, so you need to find the remainder of the division by $1000000007$ ($10^9+7$).</p><p>Nazar thought about this problem for a long time, but didn't come up with a solution. Help him solve this problem.</p></div><div class="input-specification"><p>The first line contains two integers $l$ and $r$ ($1 \leq l \leq r \leq 10^{18}$)&nbsp;— the range in which you need to find the sum.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the answer modulo $1000000007$ ($10^9+7$).</p></div>

## Input

<p>The first line contains two integers $l$ and $r$ ($1 \leq l \leq r \leq 10^{18}$)&nbsp;— the range in which you need to find the sum.</p>

## Output

<p>Print a single integer&nbsp;— the answer modulo $1000000007$ ($10^9+7$).</p>





```input1
1 3
```




```input2
5 14
```




```input3
88005553535 99999999999
```




```output1
7
```




```output2
105
```




```output3
761141116
```



## Note

<p>In the first example, the answer is the sum of the first three numbers written out ($1 + 2 + 4 = 7$).</p><p>In the second example, the numbers with numbers from $5$ to $14$: $5, 7, 9, 6, 8, 10, 12, 14, 16, 18$. Their sum is $105$.</p>
