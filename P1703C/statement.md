## Description

<div><p>Luca has a cypher made up of a sequence of $n$ wheels, each with a digit $a_i$ written on it. On the $i$-th wheel, he made $b_i$ moves. Each move is one of two types: </p><ul> <li> <span class="tex-font-style-it">up</span> move (denoted by $\texttt{U}$): it increases the $i$-th digit by $1$. After applying the up move on $9$, it becomes $0$. </li><li> <span class="tex-font-style-it">down</span> move (denoted by $\texttt{D}$): it decreases the $i$-th digit by $1$. After applying the down move on $0$, it becomes $9$. </li></ul><center> <img class="tex-graphics" src="file://Xj52zxmz.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">Example for $n=4$. The current sequence is <span class="tex-font-style-tt">0 0 0 0</span>.</span> </center><p>Luca knows the final sequence of wheels and the moves for each wheel. Help him find the original sequence and crack the cypher.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 100$)&nbsp;— the number of wheels.</p><p>The second line contains $n$ integers $a_i$ ($0 \leq a_i \leq 9$)&nbsp;— the digit shown on the $i$-th wheel after all moves have been performed.</p><p>Then $n$ lines follow, the $i$-th of which contains the integer $b_i$ ($1 \leq b_i \leq 10$) and $b_i$ characters that are either $\texttt{U}$ or $\texttt{D}$&nbsp;— the number of moves performed on the $i$-th wheel, and the moves performed. $\texttt{U}$ and $\texttt{D}$ represent an <span class="tex-font-style-it">up</span> move and a <span class="tex-font-style-it">down</span> move respectively.</p></div><div class="output-specification"><p>For each test case, output $n$ space-separated digits &nbsp;— the initial sequence of the cypher.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 100$)&nbsp;— the number of wheels.</p><p>The second line contains $n$ integers $a_i$ ($0 \leq a_i \leq 9$)&nbsp;— the digit shown on the $i$-th wheel after all moves have been performed.</p><p>Then $n$ lines follow, the $i$-th of which contains the integer $b_i$ ($1 \leq b_i \leq 10$) and $b_i$ characters that are either $\texttt{U}$ or $\texttt{D}$&nbsp;— the number of moves performed on the $i$-th wheel, and the moves performed. $\texttt{U}$ and $\texttt{D}$ represent an <span class="tex-font-style-it">up</span> move and a <span class="tex-font-style-it">down</span> move respectively.</p>

## Output

<p>For each test case, output $n$ space-separated digits &nbsp;— the initial sequence of the cypher.</p>





```input1|2,3,4,5,6,11,12,13,14,15,16,17
3
3
9 3 1
3 DDD
4 UDUU
2 DU
2
0 9
9 DDDDDDDDD
9 UUUUUUUUU
5
0 5 9 8 3
10 UUUUUUUUUU
3 UUD
8 UUDUUDDD
10 UUDUUDUDDU
4 UUUU
```




```output1
2 1 1 
9 0 
0 4 9 6 9
```



## Note

<p>In the first test case, we can prove that initial sequence was $[2,1,1]$. In that case, the following moves were performed: </p><ul> <li> On the first wheel: $2 \xrightarrow[\texttt{D}]{} 1 \xrightarrow[\texttt{D}]{} 0 \xrightarrow[\texttt{D}]{} 9$. </li><li> On the second wheel: $1 \xrightarrow[\texttt{U}]{} 2 \xrightarrow[\texttt{D}]{} 1 \xrightarrow[\texttt{U}]{} 2 \xrightarrow[\texttt{U}]{} 3$. </li><li> On the third wheel: $1 \xrightarrow[\texttt{D}]{} 0 \xrightarrow[\texttt{U}]{} 1$. </li></ul> The final sequence was $[9,3,1]$, which matches the input.
