## Description

<div><p>Let's denote a function $f(x)$ in such a way: we add $1$ to $x$, then, while there is at least one trailing zero in the resulting number, we remove that zero. For example, </p><ul> <li> $f(599) = 6$: $599 + 1 = 600 \rightarrow 60 \rightarrow 6$; </li><li> $f(7) = 8$: $7 + 1 = 8$; </li><li> $f(9) = 1$: $9 + 1 = 10 \rightarrow 1$; </li><li> $f(10099) = 101$: $10099 + 1 = 10100 \rightarrow 1010 \rightarrow 101$. </li></ul><p>We say that some number $y$ is <span class="tex-font-style-bf">reachable</span> from $x$ if we can apply function $f$ to $x$ some (possibly zero) times so that we get $y$ as a result. For example, $102$ is reachable from $10098$ because $f(f(f(10098))) = f(f(10099)) = f(101) = 102$; and any number is reachable from itself.</p><p>You are given a number $n$; your task is to count how many different numbers are reachable from $n$.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 10^9$).</p></div><div class="output-specification"><p>Print one integer: the number of different numbers that are reachable from $n$.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 10^9$).</p>

## Output

<p>Print one integer: the number of different numbers that are reachable from $n$.</p>





```input1
1098
```




```input2
10
```




```output1
20
```




```output2
19
```



## Note

<p>The numbers that are reachable from $1098$ are:</p><p>$1, 2, 3, 4, 5, 6, 7, 8, 9, 11, 12, 13, 14, 15, 16, 17, 18, 19, 1098, 1099$.</p>
