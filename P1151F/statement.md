## Description

<div><p>A girl named Sonya is studying in the scientific lyceum of the Kingdom of Kremland. The teacher of computer science (Sonya's favorite subject!) invented a task for her.</p><p>Given an array $a$ of length $n$, <span class="tex-font-style-bf">consisting only of the numbers $0$ and $1$</span>, and the number $k$. <span class="tex-font-style-bf">Exactly $k$ times</span> the following happens: </p><ul> <li> Two numbers $i$ and $j$ are chosen equiprobable such that ($1 \leq i &lt; j \leq n$). </li><li> The numbers in the $i$ and $j$ positions are swapped. </li></ul><p>Sonya's task is to find the probability that after all the operations are completed, the $a$ array will be <span class="tex-font-style-bf">sorted in non-decreasing order</span>. She turned to you for help. Help Sonya solve this problem.</p><p>It can be shown that the desired probability is either $0$ or it can be represented as $\dfrac{P}{Q}$, where $P$ and $Q$ are coprime integers and $Q \not\equiv 0~\pmod {10^9+7}$.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($2 \leq n \leq 100, 1 \leq k \leq 10^9$)&nbsp;— the length of the array $a$ and the number of operations.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 1$)&nbsp;— the description of the array $a$.</p></div><div class="output-specification"><p>If the desired probability is $0$, print $0$, otherwise print the value $P \cdot Q^{-1}$ $\pmod {10^9+7}$, where $P$ and $Q$ are defined above.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($2 \leq n \leq 100, 1 \leq k \leq 10^9$)&nbsp;— the length of the array $a$ and the number of operations.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 1$)&nbsp;— the description of the array $a$.</p>

## Output

<p>If the desired probability is $0$, print $0$, otherwise print the value $P \cdot Q^{-1}$ $\pmod {10^9+7}$, where $P$ and $Q$ are defined above.</p>





```input1
3 2
0 1 0
```




```input2
5 1
1 1 1 0 0
```




```input3
6 4
1 0 0 1 1 0
```




```output1
333333336
```




```output2
0
```




```output3
968493834
```



## Note

<p>In the first example, all possible variants of the final array $a$, after applying exactly two operations: $(0, 1, 0)$, $(0, 0, 1)$, $(1, 0, 0)$, $(1, 0, 0)$, $(0, 1, 0)$, $(0, 0, 1)$, $(0, 0, 1)$, $(1, 0, 0)$, $(0, 1, 0)$. Therefore, the answer is $\dfrac{3}{9}=\dfrac{1}{3}$.</p><p>In the second example, the array will not be sorted in non-decreasing order after one operation, therefore the answer is $0$.</p>
