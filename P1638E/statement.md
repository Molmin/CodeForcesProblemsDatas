## Description

<div><p>You have an array $a_1,a_2, \dots, a_n$. Each element initially has value $0$ and color $1$. You are also given $q$ queries to perform: </p><ul> <li> <span class="tex-font-style-tt">Color $l$ $r$ $c$</span>: Change the color of elements $a_l,a_{l+1},\cdots,a_r$ to $c$ ($1 \le l \le r \le n$, $1 \le c \le n$). </li><li> <span class="tex-font-style-tt">Add $c$ $x$</span>: Add $x$ to values of all elements $a_i$ ($1 \le i \le n$) of color $c$ ($1 \le c \le n$, $-10^9 \le x \le 10^9$). </li><li> <span class="tex-font-style-tt">Query $i$</span>: Print $a_i$ ($1 \le i \le n$). </li></ul></div><div class="input-specification"><p>The first line of input contains two integers $n$ and $q$ ($1 \le n,q \le 10^6$)&nbsp;— the length of array $a$ and the number of queries you have to perform.</p><p>Each of the next $q$ lines contains the query given in the form described in the problem statement.</p></div><div class="output-specification"><p>Print the answers to the queries of the third type on separate lines.</p></div>

## Input

<p>The first line of input contains two integers $n$ and $q$ ($1 \le n,q \le 10^6$)&nbsp;— the length of array $a$ and the number of queries you have to perform.</p><p>Each of the next $q$ lines contains the query given in the form described in the problem statement.</p>

## Output

<p>Print the answers to the queries of the third type on separate lines.</p>





```input1
5 8
Color 2 4 2
Add 2 2
Query 3
Color 4 5 3
Color 2 2 3
Add 3 3
Query 2
Query 5
```




```input2
2 7
Add 1 7
Query 1
Add 2 4
Query 2
Color 1 1 1
Add 1 1
Query 2
```




```output1
2
5
3
```




```output2
7
7
8
```



## Note

<p>The first sample test is explained below. Blue, red and green represent colors $1$, $2$ and $3$ respectively.</p><center> <img class="tex-graphics" src="file://8AUkk5Lk.png" style="max-width: 100.0%;max-height: 100.0%;" width="454px"> </center>
