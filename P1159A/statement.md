## Description

<div><p>Vasya has a pile, that consists of some number of stones. $n$ times he either took one stone from the pile or added one stone to the pile. The pile was non-empty before each operation of taking one stone from the pile.</p><p>You are given $n$ operations which Vasya has made. Find the minimal possible number of stones that can be in the pile after making these operations.</p></div><div class="input-specification"><p>The first line contains one positive integer $n$&nbsp;— the number of operations, that have been made by Vasya ($1 \leq n \leq 100$).</p><p>The next line contains the string $s$, consisting of $n$ symbols, equal to "<span class="tex-font-style-tt">-</span>" (without quotes) or "<span class="tex-font-style-tt">+</span>" (without quotes). If Vasya took the stone on $i$-th operation, $s_i$ is equal to "<span class="tex-font-style-tt">-</span>" (without quotes), if added, $s_i$ is equal to "<span class="tex-font-style-tt">+</span>" (without quotes).</p></div><div class="output-specification"><p>Print one integer&nbsp;— the minimal possible number of stones that can be in the pile after these $n$ operations.</p></div>

## Input

<p>The first line contains one positive integer $n$&nbsp;— the number of operations, that have been made by Vasya ($1 \leq n \leq 100$).</p><p>The next line contains the string $s$, consisting of $n$ symbols, equal to "<span class="tex-font-style-tt">-</span>" (without quotes) or "<span class="tex-font-style-tt">+</span>" (without quotes). If Vasya took the stone on $i$-th operation, $s_i$ is equal to "<span class="tex-font-style-tt">-</span>" (without quotes), if added, $s_i$ is equal to "<span class="tex-font-style-tt">+</span>" (without quotes).</p>

## Output

<p>Print one integer&nbsp;— the minimal possible number of stones that can be in the pile after these $n$ operations.</p>





```input1
3
---
```




```input2
4
++++
```




```input3
2
-+
```




```input4
5
++-++
```




```output1
0
```




```output2
4
```




```output3
1
```




```output4
3
```



## Note

<p>In the first test, if Vasya had $3$ stones in the pile at the beginning, after making operations the number of stones will be equal to $0$. It is impossible to have less number of piles, so the answer is $0$. Please notice, that the number of stones at the beginning can't be less, than $3$, because in this case, Vasya won't be able to take a stone on some operation (the pile will be empty).</p><p>In the second test, if Vasya had $0$ stones in the pile at the beginning, after making operations the number of stones will be equal to $4$. It is impossible to have less number of piles because after making $4$ operations the number of stones in the pile increases on $4$ stones. So, the answer is $4$.</p><p>In the third test, if Vasya had $1$ stone in the pile at the beginning, after making operations the number of stones will be equal to $1$. It can be proved, that it is impossible to have less number of stones after making the operations.</p><p>In the fourth test, if Vasya had $0$ stones in the pile at the beginning, after making operations the number of stones will be equal to $3$.</p>
