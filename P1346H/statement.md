## Description

<div><p>Alice and Bob are playing a game (yet again).</p><p>They have two sequences of segments of the coordinate axis: a sequence of $n$ <span class="tex-font-style-it">initial segments</span>: $[l_1, r_1]$, $[l_2, r_2]$, ..., $[l_n, r_n]$, and a sequence of $m$ <span class="tex-font-style-it">terminal segments</span>: $[L_1, R_1]$, $[L_2, R_2]$, ..., $[L_m, R_m]$. At the beginning of the game, they choose one of the <span class="tex-font-style-it">initial segments</span> and set it as the <span class="tex-font-style-it">current segment</span>.</p><p>Alice and Bob make alternating moves: Alice makes the first move, Bob makes the second move, Alice makes the third one, and so on. During each move, the current player <span class="tex-font-style-bf">must</span> shrink the <span class="tex-font-style-it">current segment</span> either by increasing its left endpoint by $1$, or by decreasing its right endpoint by $1$. So, if the current segment is $[c_l, c_r]$, it becomes either $[c_l + 1, c_r]$, or $[c_l, c_r - 1]$.</p><p>If at the beginning of the game or after Bob's move the <span class="tex-font-style-it">current segment</span> coincides with one of the <span class="tex-font-style-it">terminal segments</span>, Bob wins. If the <span class="tex-font-style-it">current segment</span> becomes degenerate ($c_l = c_r$), and Bob hasn't won yet, Alice wins. If the <span class="tex-font-style-it">current segment</span> coincides with one of the <span class="tex-font-style-it">terminal segments</span> after Alice's move, nothing happens — the game continues.</p><p>Both players play optimally — if they can win, they always use a strategy that leads them to victory in the minimum number of turns, and if they cannot win, they try to prolong the game, using the strategy allowing them to make the maximum possible number of moves until their defeat.</p><p>For each of the <span class="tex-font-style-it">initial segments</span> you have to determine who will win the game if this segment is chosen as the <span class="tex-font-style-it">current segment</span> at the beginning of the game. If Bob wins, you also have to calculate the number of moves Alice will make before her defeat.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 2 \cdot 10^5$) — the number of <span class="tex-font-style-it">initial segments</span> and <span class="tex-font-style-it">terminal segments</span>, respectively.</p><p>Then $n$ lines follow, the $i$-th line contains two integers $l_i$ and $r_i$ ($1 \le l_i &lt; r_i \le 10^6$) — the endpoints of the $i$-th <span class="tex-font-style-it">initial segment</span>.</p><p>Then $m$ lines follow, the $i$-th line contains two integers $L_i$ and $R_i$ ($1 \le L_i &lt; R_i \le 10^6$) — the endpoints of the $i$-th <span class="tex-font-style-it">terminal segment</span>.</p><p><span class="tex-font-style-bf">Note that some of the segments given in the input may coincide</span>.</p></div><div class="output-specification"><p>Print $n$ integers, the $i$-th of them should describe the result of the game if the $i$-th <span class="tex-font-style-it">initial segment</span> is chosen at the beginning of the game:</p><ul> <li> if Alice wins, print $-1$; </li><li> if Bob wins, print the number of moves Alice will make before she is defeated. </li></ul></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 2 \cdot 10^5$) — the number of <span class="tex-font-style-it">initial segments</span> and <span class="tex-font-style-it">terminal segments</span>, respectively.</p><p>Then $n$ lines follow, the $i$-th line contains two integers $l_i$ and $r_i$ ($1 \le l_i &lt; r_i \le 10^6$) — the endpoints of the $i$-th <span class="tex-font-style-it">initial segment</span>.</p><p>Then $m$ lines follow, the $i$-th line contains two integers $L_i$ and $R_i$ ($1 \le L_i &lt; R_i \le 10^6$) — the endpoints of the $i$-th <span class="tex-font-style-it">terminal segment</span>.</p><p><span class="tex-font-style-bf">Note that some of the segments given in the input may coincide</span>.</p>

## Output

<p>Print $n$ integers, the $i$-th of them should describe the result of the game if the $i$-th <span class="tex-font-style-it">initial segment</span> is chosen at the beginning of the game:</p><ul> <li> if Alice wins, print $-1$; </li><li> if Bob wins, print the number of moves Alice will make before she is defeated. </li></ul>





```input1
1 1
4 7
4 7
```




```input2
1 2
2 5
2 4
3 5
```




```input3
2 1
1 5
1 4
2 3
```




```output1
0
```




```output2
-1
```




```output3
-1 1
```


