## Description

<div><p>You are given an array $a$ of length $n$ that consists of zeros and ones.</p><p>You can perform the following operation multiple times. The operation consists of two steps: </p><ol> <li> Choose three integers $1 \le x &lt; y &lt; z \le n$, that form an arithmetic progression ($y - x = z - y$). </li><li> Flip the values $a_x, a_y, a_z$ (i.e. change $1$ to $0$, change $0$ to $1$). </li></ol><p>Determine if it is possible to make all elements of the array equal to zero. If yes, print the operations that lead the the all-zero state. Your solution should not contain more than $(\lfloor \frac{n}{3} \rfloor + 12)$ operations. Here $\lfloor q \rfloor$ denotes the number $q$ rounded down. We can show that it is possible to make all elements equal to zero in no more than this number of operations whenever it is possible to do so at all.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($3 \le n \le 10^5$) — the length of the array.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 1$) — the elements of the array.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" (without quotes) if the answer exists, otherwise print "<span class="tex-font-style-tt">NO</span>" (without quotes). You can print each letter in any case (upper or lower).</p><p>If there is an answer, in the second line print an integer $m$ ($0 \le m \le (\lfloor \frac{n}{3} \rfloor + 12)$) — the number of operations in your answer.</p><p>After that in ($i + 2$)-th line print the $i$-th operations&nbsp;— the integers $x_i, y_i, z_i$. You can print them in arbitrary order.</p></div>

## Input

<p>The first line contains a single integer $n$ ($3 \le n \le 10^5$) — the length of the array.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 1$) — the elements of the array.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" (without quotes) if the answer exists, otherwise print "<span class="tex-font-style-tt">NO</span>" (without quotes). You can print each letter in any case (upper or lower).</p><p>If there is an answer, in the second line print an integer $m$ ($0 \le m \le (\lfloor \frac{n}{3} \rfloor + 12)$) — the number of operations in your answer.</p><p>After that in ($i + 2$)-th line print the $i$-th operations&nbsp;— the integers $x_i, y_i, z_i$. You can print them in arbitrary order.</p>





```input1
5
1 1 0 1 1

```




```input2
3
0 1 0

```




```output1
YES
2
1 3 5
2 3 4

```




```output2
NO

```



## Note

<p>In the first sample the shown output corresponds to the following solution: </p><ul> <li> <span class="tex-font-style-tt">1 1 0 1 1</span> (initial state); </li><li> <span class="tex-font-style-tt">0 1 1 1 0</span> (the flipped positions are the first, the third and the fifth elements); </li><li> <span class="tex-font-style-tt">0 0 0 0 0</span> (the flipped positions are the second, the third and the fourth elements). </li></ul><p>Other answers are also possible. In this test the number of operations should not exceed $\lfloor \frac{5}{3} \rfloor + 12 = 1 + 12 = 13$.</p><p>In the second sample the only available operation is to flip all the elements. This way it is only possible to obtain the arrays <span class="tex-font-style-tt">0 1 0</span> and <span class="tex-font-style-tt">1 0 1</span>, but it is impossible to make all elements equal to zero.</p>
