## Description

<div><p>Adilbek's house is located on a street which can be represented as the OX axis. This street is really dark, so Adilbek wants to install some post lamps to illuminate it. Street has $n$ positions to install lamps, they correspond to the integer numbers from $0$ to $n - 1$ on the OX axis. However, some positions are blocked and no post lamp can be placed there.</p><p>There are post lamps of different types which differ only by their power. When placed in position $x$, post lamp of power $l$ illuminates the segment $[x; x + l]$. The power of each post lamp is always a positive integer number.</p><p>The post lamp shop provides an infinite amount of lamps of each type from power $1$ to power $k$. Though each customer is only allowed to order post lamps of <span class="tex-font-style-it">exactly one</span> type. Post lamps of power $l$ cost $a_l$ each.</p><p>What is the minimal total cost of the post lamps of <span class="tex-font-style-it">exactly one</span> type Adilbek can buy to illuminate the entire segment $[0; n]$ of the street? If some lamps illuminate any other segment of the street, Adilbek does not care, so, for example, he may place a lamp of power $3$ in position $n - 1$ (even though its illumination zone doesn't completely belong to segment $[0; n]$).</p></div><div class="input-specification"><p>The first line contains three integer numbers $n$, $m$ and $k$ ($1 \le k \le n \le 10^6$, $0 \le m \le n$) — the length of the segment of the street Adilbek wants to illuminate, the number of the blocked positions and the maximum power of the post lamp available.</p><p>The second line contains $m$ integer numbers $s_1, s_2, \dots, s_m$ ($0 \le s_1 &lt; s_2 &lt; \dots s_m &lt; n$) — the blocked positions.</p><p>The third line contains $k$ integer numbers $a_1, a_2, \dots, a_k$ ($1 \le a_i \le 10^6$) — the costs of the post lamps.</p></div><div class="output-specification"><p>Print the minimal total cost of the post lamps of <span class="tex-font-style-it">exactly one</span> type Adilbek can buy to illuminate the entire segment $[0; n]$ of the street.</p><p>If illumintaing the entire segment $[0; n]$ is impossible, print <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains three integer numbers $n$, $m$ and $k$ ($1 \le k \le n \le 10^6$, $0 \le m \le n$) — the length of the segment of the street Adilbek wants to illuminate, the number of the blocked positions and the maximum power of the post lamp available.</p><p>The second line contains $m$ integer numbers $s_1, s_2, \dots, s_m$ ($0 \le s_1 &lt; s_2 &lt; \dots s_m &lt; n$) — the blocked positions.</p><p>The third line contains $k$ integer numbers $a_1, a_2, \dots, a_k$ ($1 \le a_i \le 10^6$) — the costs of the post lamps.</p>

## Output

<p>Print the minimal total cost of the post lamps of <span class="tex-font-style-it">exactly one</span> type Adilbek can buy to illuminate the entire segment $[0; n]$ of the street.</p><p>If illumintaing the entire segment $[0; n]$ is impossible, print <span class="tex-font-style-tt">-1</span>.</p>





```input1
6 2 3
1 3
1 2 3

```




```input2
4 3 4
1 2 3
1 10 100 1000

```




```input3
5 1 5
0
3 3 3 3 3

```




```input4
7 4 3
2 4 5 6
3 14 15

```




```output1
6

```




```output2
1000

```




```output3
-1

```




```output4
-1

```


