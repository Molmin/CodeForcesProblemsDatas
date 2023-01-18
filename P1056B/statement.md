## Description

<div><p>Arkady and his friends love playing checkers on an $n \times n$ field. The rows and the columns of the field are enumerated from $1$ to $n$.</p><p>The friends have recently won a championship, so Arkady wants to please them with some candies. Remembering an old parable (but not its moral), Arkady wants to give to his friends one set of candies per each cell of the field: the set of candies for cell $(i, j)$ will have exactly $(i^2 + j^2)$ candies of unique type.</p><p>There are $m$ friends who deserve the present. How many of these $n \times n$ sets of candies can be split equally into $m$ parts without cutting a candy into pieces? Note that each set has to be split independently since the types of candies in different sets are different.</p></div><div class="input-specification"><p>The only line contains two integers $n$ and $m$ ($1 \le n \le 10^9$, $1 \le m \le 1000$)&nbsp;— the size of the field and the number of parts to split the sets into.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the number of sets that can be split equally.</p></div>

## Input

<p>The only line contains two integers $n$ and $m$ ($1 \le n \le 10^9$, $1 \le m \le 1000$)&nbsp;— the size of the field and the number of parts to split the sets into.</p>

## Output

<p>Print a single integer&nbsp;— the number of sets that can be split equally.</p>





```input1
3 3
```




```input2
6 5
```




```input3
1000000000 1
```




```output1
1
```




```output2
13
```




```output3
1000000000000000000
```



## Note

<p>In the first example, only the set for cell $(3, 3)$ can be split equally ($3^2 + 3^2 = 18$, which is divisible by $m=3$).</p><p>In the second example, the sets for the following cells can be divided equally: </p><ul> <li> $(1, 2)$ and $(2, 1)$, since $1^2 + 2^2 = 5$, which is divisible by $5$; </li><li> $(1, 3)$ and $(3, 1)$; </li><li> $(2, 4)$ and $(4, 2)$; </li><li> $(2, 6)$ and $(6, 2)$; </li><li> $(3, 4)$ and $(4, 3)$; </li><li> $(3, 6)$ and $(6, 3)$; </li><li> $(5, 5)$. </li></ul><p>In the third example, sets in all cells can be divided equally, since $m = 1$.</p>
