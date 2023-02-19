## Description

<div><p><span class="tex-font-style-bf">Note that the memory limit is unusual.</span></p><p>You are given an integer $n$ and two sequences $a_1, a_2, \dots, a_n$ and $b_1, b_2, \dots, b_n$.</p><p>Let's call a set of integers $S$ such that $S \subseteq \{1, 2, 3, \dots, n\}$ <span class="tex-font-style-it">strange</span>, if, for every element $i$ of $S$, the following condition is met: for every $j \in [1, i - 1]$, if $a_j$ divides $a_i$, then $j$ is also included in $S$. An empty set is always <span class="tex-font-style-it">strange</span>.</p><p>The <span class="tex-font-style-it">cost</span> of the set $S$ is $\sum\limits_{i \in S} b_i$. You have to calculate the maximum possible <span class="tex-font-style-it">cost</span> of a <span class="tex-font-style-it">strange</span> set.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 3000$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 100$).</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n$ ($-10^5 \le b_i \le 10^5$).</p></div><div class="output-specification"><p>Print one integer — the maximum <span class="tex-font-style-it">cost</span> of a <span class="tex-font-style-it">strange</span> set.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 3000$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 100$).</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n$ ($-10^5 \le b_i \le 10^5$).</p>

## Output

<p>Print one integer — the maximum <span class="tex-font-style-it">cost</span> of a <span class="tex-font-style-it">strange</span> set.</p>





```input1
9
4 7 3 4 5 6 7 8 13
-2 3 -19 5 -6 7 -8 9 1
```




```input2
2
42 42
-37 13
```




```input3
2
42 42
13 -37
```




```output1
16
```




```output2
0
```




```output3
13
```



## Note

<p>The <span class="tex-font-style-it">strange</span> set with the maximum <span class="tex-font-style-it">cost</span> in the first example is $\{1, 2, 4, 8, 9\}$.</p><p>The <span class="tex-font-style-it">strange</span> set with the maximum <span class="tex-font-style-it">cost</span> in the second example is empty.</p>
