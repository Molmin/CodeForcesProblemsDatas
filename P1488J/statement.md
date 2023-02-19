## Description

<div><p>Your friend is running a flower shop. In order to be prepared for the next holidays (when, as usual, sales skyrocket) she asked you to write her a special program that will help to analyze the stocks she has.</p><p>There are $n$ different types of flowers she can order and each flower of the type $i$ costs $w_i$. The last holidays were a great success, she sold all flowers she had, so right now all her stocks are empty.</p><p>From this point, she starts routine operations of ordering and selling flowers, while trying to analyze what she has at hand. All of this can be represented as $m$ queries of three types: </p><ul> <li> "<span class="tex-font-style-tt">$1$ $i$ $c$</span>"&nbsp;— she bought $c$ flowers of type $i$; </li><li> "<span class="tex-font-style-tt">$2$ $i$ $c$</span>"&nbsp;— she disposed of $c$ flowers of type $i$; </li><li> "<span class="tex-font-style-tt">$3$ $l$ $r$ $k$</span>"&nbsp;— how many variants of bouquets she can make using only flowers of types $l, l + 1, \dots, r$ with the total cost no more than $k$. For simplicity, you can think that a bouquet is a multiset of flowers, and two bouquets are different if they are different as multisets. The cost of a bouquet is the sum of all flowers it has. </li></ul><p>Help your friend and write the program that can process all these queries.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n \le 1000$; $1 \le m \le 1000$)&nbsp;— the number of flower types and the number of queries.</p><p>The second line contains $n$ integers $w_1, w_2, \dots, w_n$ ($1 \le w_i \le 1000$)&nbsp;— the cost of one flower of each type.</p><p>The next $m$ lines contains queries&nbsp;— one per line. Each query has one of three types: </p><ul> <li> <span class="tex-font-style-tt">$1$ $i$ $c$</span> ($1 \le i \le n$; $1 \le c \le 5000$); </li><li> <span class="tex-font-style-tt">$2$ $i$ $c$</span> ($1 \le i \le n$; $1 \le c \le 5000$). It's guaranteed that there are at least $c$ flowers of type $i$ at this moment; </li><li> <span class="tex-font-style-tt">$3$ $l$ $r$ $k$</span> ($1 \le l \le r \le n$; $1 \le k \le 5000$) </li></ul><p><span class="tex-font-style-bf">It's guaranteed that the total cost of all flowers in stock after each query doesn't exceed $5000$</span>.</p></div><div class="output-specification"><p>For each query of the third type, print how many variants of bouquets she can make using only flowers of types $l, l + 1, \dots, r$ with the total cost no more than $k$. Since the answer may be too large, print it modulo $998\,244\,353$.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n \le 1000$; $1 \le m \le 1000$)&nbsp;— the number of flower types and the number of queries.</p><p>The second line contains $n$ integers $w_1, w_2, \dots, w_n$ ($1 \le w_i \le 1000$)&nbsp;— the cost of one flower of each type.</p><p>The next $m$ lines contains queries&nbsp;— one per line. Each query has one of three types: </p><ul> <li> <span class="tex-font-style-tt">$1$ $i$ $c$</span> ($1 \le i \le n$; $1 \le c \le 5000$); </li><li> <span class="tex-font-style-tt">$2$ $i$ $c$</span> ($1 \le i \le n$; $1 \le c \le 5000$). It's guaranteed that there are at least $c$ flowers of type $i$ at this moment; </li><li> <span class="tex-font-style-tt">$3$ $l$ $r$ $k$</span> ($1 \le l \le r \le n$; $1 \le k \le 5000$) </li></ul><p><span class="tex-font-style-bf">It's guaranteed that the total cost of all flowers in stock after each query doesn't exceed $5000$</span>.</p>

## Output

<p>For each query of the third type, print how many variants of bouquets she can make using only flowers of types $l, l + 1, \dots, r$ with the total cost no more than $k$. Since the answer may be too large, print it modulo $998\,244\,353$.</p>





```input1
5 12
1 2 3 2 1
1 1 5
1 2 3
1 3 1
3 1 5 10
3 4 5 100
1 4 4
1 5 1
3 2 5 7
3 1 1 3
3 1 5 100
2 1 5
3 1 5 100
```




```output1
40
0
28
3
479
79
```


