## Description

<div><p>You have unlimited number of coins with values $1, 2, \ldots, n$. You want to select some set of coins having the total value of $S$. </p><p>It is allowed to have multiple coins with the same value in the set. What is the minimum number of coins required to get sum $S$?</p></div><div class="input-specification"><p>The only line of the input contains two integers $n$ and $S$ ($1 \le n \le 100\,000$, $1 \le S \le 10^9$)</p></div><div class="output-specification"><p>Print exactly one integer&nbsp;— the minimum number of coins required to obtain sum $S$.</p></div>

## Input

<p>The only line of the input contains two integers $n$ and $S$ ($1 \le n \le 100\,000$, $1 \le S \le 10^9$)</p>

## Output

<p>Print exactly one integer&nbsp;— the minimum number of coins required to obtain sum $S$.</p>





```input1
5 11

```




```input2
6 16

```




```output1
3
```




```output2
3
```



## Note

<p>In the first example, some of the possible ways to get sum $11$ with $3$ coins are: </p><ul> <li> $(3, 4, 4)$</li><li> $(2, 4, 5)$</li><li> $(1, 5, 5)$</li><li> $(3, 3, 5)$ </li></ul><p>It is impossible to get sum $11$ with less than $3$ coins.</p><p>In the second example, some of the possible ways to get sum $16$ with $3$ coins are: </p><ul> <li> $(5, 5, 6)$</li><li> $(4, 6, 6)$ </li></ul><p>It is impossible to get sum $16$ with less than $3$ coins.</p>
