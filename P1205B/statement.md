## Description

<div><p>You are given $n$ integer numbers $a_1, a_2, \dots, a_n$. Consider graph on $n$ nodes, in which nodes $i$, $j$ ($i\neq j$) are connected if and only if, $a_i$ AND $a_j\neq 0$, where AND denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#AND">bitwise AND operation</a>.</p><p>Find the length of the shortest cycle in this graph or determine that it doesn't have cycles at all.</p></div><div class="input-specification"><p>The first line contains one integer $n$ $(1 \le n \le 10^5)$&nbsp;— number of numbers.</p><p>The second line contains $n$ integer numbers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 10^{18}$).</p></div><div class="output-specification"><p>If the graph doesn't have any cycles, output $-1$. Else output the length of the shortest cycle.</p></div>

## Input

<p>The first line contains one integer $n$ $(1 \le n \le 10^5)$&nbsp;— number of numbers.</p><p>The second line contains $n$ integer numbers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 10^{18}$).</p>

## Output

<p>If the graph doesn't have any cycles, output $-1$. Else output the length of the shortest cycle.</p>





```input1
4
3 6 28 9
```




```input2
5
5 12 9 16 48
```




```input3
4
1 2 4 8
```




```output1
4
```




```output2
3
```




```output3
-1
```



## Note

<p>In the first example, the shortest cycle is $(9, 3, 6, 28)$.</p><p>In the second example, the shortest cycle is $(5, 12, 9)$.</p><p>The graph has no cycles in the third example.</p>
