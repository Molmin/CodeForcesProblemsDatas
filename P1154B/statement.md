## Description

<div><p>You are given a sequence $a_1, a_2, \dots, a_n$ consisting of $n$ integers.</p><p>You can choose any non-negative integer $D$ (i.e. $D \ge 0$), and for each $a_i$ you can:</p><ul> <li> add $D$ (only once), i. e. perform $a_i := a_i + D$, or </li><li> subtract $D$ (only once), i. e. perform $a_i := a_i - D$, or </li><li> leave the value of $a_i$ unchanged. </li></ul><p>It is possible that after an operation the value $a_i$ becomes negative.</p><p>Your goal is to choose such <span class="tex-font-style-bf">minimum non-negative integer</span> $D$ and perform changes in such a way, that all $a_i$ are equal (i.e. $a_1=a_2=\dots=a_n$).</p><p>Print the required $D$ or, if it is impossible to choose such value $D$, print <span class="tex-font-style-tt">-1</span>.</p><p>For example, for array $[2, 8]$ the value $D=3$ is minimum possible because you can obtain the array $[5, 5]$ if you will add $D$ to $2$ and subtract $D$ from $8$. And for array $[1, 4, 7, 7]$ the value $D=3$ is also minimum possible. You can add it to $1$ and subtract it from $7$ and obtain the array $[4, 4, 4, 4]$.</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($1 \le n \le 100$) — the number of elements in $a$.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 100$) — the sequence $a$.</p></div><div class="output-specification"><p>Print one integer — the <span class="tex-font-style-bf">minimum non-negative integer</span> value $D$ such that if you add this value to some $a_i$, subtract this value from some $a_i$ and leave some $a_i$ without changes, all obtained values become equal.</p><p>If it is impossible to choose such value $D$, print <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($1 \le n \le 100$) — the number of elements in $a$.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 100$) — the sequence $a$.</p>

## Output

<p>Print one integer — the <span class="tex-font-style-bf">minimum non-negative integer</span> value $D$ such that if you add this value to some $a_i$, subtract this value from some $a_i$ and leave some $a_i$ without changes, all obtained values become equal.</p><p>If it is impossible to choose such value $D$, print <span class="tex-font-style-tt">-1</span>.</p>





```input1
6
1 4 4 7 4 1
```




```input2
5
2 2 5 2 5
```




```input3
4
1 3 3 7
```




```input4
2
2 8
```




```output1
3
```




```output2
3
```




```output3
-1
```




```output4
3
```


