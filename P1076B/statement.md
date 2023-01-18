## Description

<div><p>You are given an integer number $n$. The following algorithm is applied to it:</p><ol> <li> if $n = 0$, then end algorithm; </li><li> find the smallest <span class="tex-font-style-bf">prime</span> divisor $d$ of $n$; </li><li> subtract $d$ from $n$ and go to step $1$. </li></ol><p>Determine the number of subtrations the algorithm will make.</p></div><div class="input-specification"><p>The only line contains a single integer $n$ ($2 \le n \le 10^{10}$).</p></div><div class="output-specification"><p>Print a single integer — the number of subtractions the algorithm will make.</p></div>

## Input

<p>The only line contains a single integer $n$ ($2 \le n \le 10^{10}$).</p>

## Output

<p>Print a single integer — the number of subtractions the algorithm will make.</p>





```input1
5
```




```input2
4
```




```output1
1
```




```output2
2
```



## Note

<p>In the first example $5$ is the smallest prime divisor, thus it gets subtracted right away to make a $0$.</p><p>In the second example $2$ is the smallest prime divisor at both steps.</p>
