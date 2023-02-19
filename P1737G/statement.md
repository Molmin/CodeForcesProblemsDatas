## Description

<div><p></p><table class="tex-tabular"><tbody><tr><td class="tex-tabular-text-align-left"><img class="tex-graphics" src="file://pqgHrp1V.png" style="max-width: 100.0%;max-height: 100.0%;"></td><td class="tex-tabular-text-align-left"><span class="tex-font-style-it">DTL engineers love partying in the weekend. Ela does, too! Unfortunately, she didn't know how to dance yet. Therefore, she decided to take a dancing class.</span></td></tr></tbody></table><p></p><p>There are $n$ students in the dancing class, including Ela. In the final project, $n$ students will participate in a choreography described below.</p><p>$n$ students are positioned on the positive side of the $Ox$-axis. The $i$-th dancer is located at $a_i &gt; 0$. Some dancers will change positions during the dance (we'll call them <span class="tex-font-style-it">movable dancers</span>), and others will stay in the same place during a choreography (we'll call them <span class="tex-font-style-it">immovable dancers</span>). We distinguish the dancers using a binary string $s$ of length $n$: if $s_i$ equals <span class="tex-font-style-tt">'1'</span>, then the $i$-th dancer is movable, otherwise the $i$-th dancer is immovable.</p><p>Let's call the <span class="tex-font-style-it">"positive energy value"</span> of the choreography $d &gt; 0$. The dancers will perform <span class="tex-font-style-it">"movements"</span> based on this value.</p><p>Each minute after the dance begins, the movable dancer with the <span class="tex-font-style-bf">smallest</span> $x$-coordinate will start moving to the right and initiate a <span class="tex-font-style-it">"movement"</span>. At the beginning of the <span class="tex-font-style-it">movement</span>, the dancer's energy level will be initiated equally to the positive energy value of the choreography, which is $d$. Each time they move from some $y$ to $y+1$, the energy level will be decreased by $1$. At some point, the dancer might meet other fellow dancers in the same coordinates. If it happens, then the energy level of the dancer will be increased by $1$. A dancer will stop moving to the right when his energy level reaches $0$, and he doesn't share a position with another dancer.</p><p>The dancers are very well-trained, and each <span class="tex-font-style-it">"movement"</span> will end before the next minute begins.</p><p>To show her understanding of this choreography, Ela has to answer $q$ queries, each consisting of two integers $k$ and $m$. The answer to this query is the coordinate of the $m$-th dancer <span class="tex-font-style-bf">of both types</span> from the left at $k$-th minute after the choreography begins. In other words, denote $x_{k, 1}, x_{k, 2}, \dots, x_{k, n}$ as the sorted coordinates of the dancers at $k$-th minute from the beginning, you need to print $x_{k, m}$.</p></div><div class="input-specification"><p>The first line contains three integers $n$, $d$ and $q$ ($1 \le n \le 10^5$; $1 \le d \le 10^9$; $1 \le q \le 10^5$) — the number of dancers, the positive energy value of the choreography, and the number of queries.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_1 &lt; a_2 &lt; \dots &lt; a_n \le 10^9$) — the coordinates of each dancer.</p><p>The third line contains a binary string $s$ of length $n$ — the movability of each dancer. Each character is either <span class="tex-font-style-tt">'0'</span> or <span class="tex-font-style-tt">'1'</span>. It is guaranteed that $s$ contains at least one character <span class="tex-font-style-tt">'1'</span>.</p><p>Then $q$ lines follow, the $i$-th of them contains two integers $k_i$ and $m_i$ ($1 \le k_i \le 10^9$, $1 \le m_i \le n$) — the content of each query.</p></div><div class="output-specification"><p>Output $q$ lines, each contains a single integer — the answer for the corresponding query.</p></div>

## Input

<p>The first line contains three integers $n$, $d$ and $q$ ($1 \le n \le 10^5$; $1 \le d \le 10^9$; $1 \le q \le 10^5$) — the number of dancers, the positive energy value of the choreography, and the number of queries.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_1 &lt; a_2 &lt; \dots &lt; a_n \le 10^9$) — the coordinates of each dancer.</p><p>The third line contains a binary string $s$ of length $n$ — the movability of each dancer. Each character is either <span class="tex-font-style-tt">'0'</span> or <span class="tex-font-style-tt">'1'</span>. It is guaranteed that $s$ contains at least one character <span class="tex-font-style-tt">'1'</span>.</p><p>Then $q$ lines follow, the $i$-th of them contains two integers $k_i$ and $m_i$ ($1 \le k_i \le 10^9$, $1 \le m_i \le n$) — the content of each query.</p>

## Output

<p>Output $q$ lines, each contains a single integer — the answer for the corresponding query.</p>





```input1
4 3 8
1 3 6 7
1011
1 1
1 2
1 3
1 4
2 1
2 2
2 3
2 4
```




```input2
1 1 5
2
1
1 1
2 1
3 1
4 1
5 1
```




```output1
3
5
6
7
3
6
7
10
```




```output2
3
4
5
6
7
```



## Note

<p>Let's consider the first example test case.</p><p>In the first minute, $1$ is the lowest coordinate between movable dancers. The energy level is initiated with $3$. Then the following happens: </p><ul> <li> The dancer moves from $1$ to $2$. The energy level decreased to $2$. </li><li> The dancer moves from $2$ to $3$. The energy level decreased to $1$, then increased to $2$ when she met another dancer at $3$. </li><li> The dancer moves from $3$ to $4$. The energy level decreased to $1$. </li><li> The dancer moves from $4$ to $5$. The energy level decreased to $0$. </li></ul><p>At the end of the first minute, the sorted coordinates of the dancers become $[3, 5, 6, 7]$, and their respective movability is <span class="tex-font-style-tt">'0111'</span>.</p><p>In the second minute, $5$ is the lowest coordinate between movable dancers. The energy level is initiated with $3$. Then the following happens: </p><ul> <li> The dancer moves from $5$ to $6$. The energy level decreased to $2$, then increased to $3$ when she met another dancer at $6$. </li><li> The dancer moves from $6$ to $7$. The energy level decreased to $2$, then increased to $3$ when she met another dancer at $7$. </li><li> The dancer moves from $7$ to $8$. The energy level decreased to $2$. </li><li> The dancer moves from $8$ to $9$. The energy level decreased to $1$. </li><li> The dancer moves from $9$ to $10$. The energy level decreased to $0$. </li></ul><p>At the end of the second minute, the sorted coordinates of the dancers become $[3, 6, 7, 10]$, and their respective movability is <span class="tex-font-style-tt">'0111'</span>.</p>
