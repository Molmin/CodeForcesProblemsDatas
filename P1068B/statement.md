## Description

<div><p>Ivan has number $b$. He is sorting through the numbers $a$ from $1$ to $10^{18}$, and for every $a$ writes $\frac{[a, \,\, b]}{a}$ on blackboard. Here $[a, \,\, b]$ stands for least common multiple of $a$ and $b$. Ivan is very lazy, that's why this task bored him soon. But he is interested in how many different numbers he would write on the board if he would finish the task. Help him to find the quantity of different numbers he would write on the board.</p></div><div class="input-specification"><p>The only line contains one integer&nbsp;— $b$ $(1 \le b \le 10^{10})$.</p></div><div class="output-specification"><p>Print one number&nbsp;— answer for the problem.</p></div>

## Input

<p>The only line contains one integer&nbsp;— $b$ $(1 \le b \le 10^{10})$.</p>

## Output

<p>Print one number&nbsp;— answer for the problem.</p>





```input1
1

```




```input2
2

```




```output1
1
```




```output2
2
```



## Note

<p>In the first example $[a, \,\, 1] = a$, therefore $\frac{[a, \,\, b]}{a}$ is always equal to $1$.</p><p>In the second example $[a, \,\, 2]$ can be equal to $a$ or $2 \cdot a$ depending on parity of $a$. $\frac{[a, \,\, b]}{a}$ can be equal to $1$ and $2$.</p>
