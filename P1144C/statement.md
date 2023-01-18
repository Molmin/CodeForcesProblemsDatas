## Description

<div><p>Two integer sequences existed initially — one of them was <span class="tex-font-style-bf">strictly</span> increasing, and the other one — <span class="tex-font-style-bf">strictly</span> decreasing.</p><p>Strictly increasing sequence is a sequence of integers $[x_1 &lt; x_2 &lt; \dots &lt; x_k]$. And strictly decreasing sequence is a sequence of integers $[y_1 &gt; y_2 &gt; \dots &gt; y_l]$. Note that the empty sequence and the sequence consisting of one element can be considered as increasing or decreasing.</p><p>They were merged into one sequence $a$. After that sequence $a$ got shuffled. For example, some of the possible resulting sequences $a$ for an increasing sequence $[1, 3, 4]$ and a decreasing sequence $[10, 4, 2]$ are sequences $[1, 2, 3, 4, 4, 10]$ or $[4, 2, 1, 10, 4, 3]$.</p><p>This shuffled sequence $a$ is given in the input.</p><p>Your task is to find <span class="tex-font-style-bf">any</span> two suitable initial sequences. One of them should be <span class="tex-font-style-bf">strictly</span> increasing and the other one — <span class="tex-font-style-bf">strictly</span> decreasing. Note that the empty sequence and the sequence consisting of one element can be considered as increasing or decreasing.</p><p>If there is a contradiction in the input and it is impossible to split the given sequence $a$ to increasing and decreasing sequences, print "<span class="tex-font-style-tt">NO</span>".</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of elements in $a$.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 2 \cdot 10^5$), where $a_i$ is the $i$-th element of $a$.</p></div><div class="output-specification"><p>If there is a contradiction in the input and it is impossible to split the given sequence $a$ to increasing and decreasing sequences, print "<span class="tex-font-style-tt">NO</span>" in the first line.</p><p>Otherwise print "<span class="tex-font-style-tt">YES</span>" in the first line and <span class="tex-font-style-bf">any</span> two suitable sequences. Note that the empty sequence and the sequence consisting of one element can be considered as increasing or decreasing.</p><p>In the second line print $n_i$ — the number of elements in the <span class="tex-font-style-bf">strictly increasing</span> sequence. $n_i$ can be zero, in this case the increasing sequence is empty.</p><p>In the third line print $n_i$ integers $inc_1, inc_2, \dots, inc_{n_i}$ in the <span class="tex-font-style-bf">increasing</span> order of its values ($inc_1 &lt; inc_2 &lt; \dots &lt; inc_{n_i}$) — the <span class="tex-font-style-bf">strictly increasing</span> sequence itself. You can keep this line empty if $n_i = 0$ (or just print the empty line).</p><p>In the fourth line print $n_d$ — the number of elements in the <span class="tex-font-style-bf">strictly decreasing</span> sequence. $n_d$ can be zero, in this case the decreasing sequence is empty.</p><p>In the fifth line print $n_d$ integers $dec_1, dec_2, \dots, dec_{n_d}$ in the <span class="tex-font-style-bf">decreasing</span> order of its values ($dec_1 &gt; dec_2 &gt; \dots &gt; dec_{n_d}$) — the <span class="tex-font-style-bf">strictly decreasing</span> sequence itself. You can keep this line empty if $n_d = 0$ (or just print the empty line).</p><p>$n_i + n_d$ should be equal to $n$ and the union of printed sequences should be a permutation of the given sequence (in case of "<span class="tex-font-style-tt">YES</span>" answer).</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of elements in $a$.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 2 \cdot 10^5$), where $a_i$ is the $i$-th element of $a$.</p>

## Output

<p>If there is a contradiction in the input and it is impossible to split the given sequence $a$ to increasing and decreasing sequences, print "<span class="tex-font-style-tt">NO</span>" in the first line.</p><p>Otherwise print "<span class="tex-font-style-tt">YES</span>" in the first line and <span class="tex-font-style-bf">any</span> two suitable sequences. Note that the empty sequence and the sequence consisting of one element can be considered as increasing or decreasing.</p><p>In the second line print $n_i$ — the number of elements in the <span class="tex-font-style-bf">strictly increasing</span> sequence. $n_i$ can be zero, in this case the increasing sequence is empty.</p><p>In the third line print $n_i$ integers $inc_1, inc_2, \dots, inc_{n_i}$ in the <span class="tex-font-style-bf">increasing</span> order of its values ($inc_1 &lt; inc_2 &lt; \dots &lt; inc_{n_i}$) — the <span class="tex-font-style-bf">strictly increasing</span> sequence itself. You can keep this line empty if $n_i = 0$ (or just print the empty line).</p><p>In the fourth line print $n_d$ — the number of elements in the <span class="tex-font-style-bf">strictly decreasing</span> sequence. $n_d$ can be zero, in this case the decreasing sequence is empty.</p><p>In the fifth line print $n_d$ integers $dec_1, dec_2, \dots, dec_{n_d}$ in the <span class="tex-font-style-bf">decreasing</span> order of its values ($dec_1 &gt; dec_2 &gt; \dots &gt; dec_{n_d}$) — the <span class="tex-font-style-bf">strictly decreasing</span> sequence itself. You can keep this line empty if $n_d = 0$ (or just print the empty line).</p><p>$n_i + n_d$ should be equal to $n$ and the union of printed sequences should be a permutation of the given sequence (in case of "<span class="tex-font-style-tt">YES</span>" answer).</p>





```input1
7
7 2 7 3 3 1 4
```




```input2
5
4 3 1 5 3
```




```input3
5
1 1 2 1 2
```




```input4
5
0 1 2 3 4
```




```output1
YES
2
3 7 
5
7 4 3 2 1
```




```output2
YES
1
3 
4
5 4 3 1
```




```output3
NO
```




```output4
YES
0

5
4 3 2 1 0
```


