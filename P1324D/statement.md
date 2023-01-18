## Description

<div><p>The next lecture in a high school requires two topics to be discussed. The $i$-th topic is interesting by $a_i$ units for the teacher and by $b_i$ units for the students.</p><p>The pair of topics $i$ and $j$ ($i &lt; j$) is called <span class="tex-font-style-bf">good</span> if $a_i + a_j &gt; b_i + b_j$ (i.e. it is more interesting for the teacher).</p><p>Your task is to find the number of <span class="tex-font-style-bf">good</span> pairs of topics.</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the number of topics.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$), where $a_i$ is the interestingness of the $i$-th topic for the teacher.</p><p>The third line of the input contains $n$ integers $b_1, b_2, \dots, b_n$ ($1 \le b_i \le 10^9$), where $b_i$ is the interestingness of the $i$-th topic for the students.</p></div><div class="output-specification"><p>Print one integer — the number of <span class="tex-font-style-bf">good</span> pairs of topic.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the number of topics.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$), where $a_i$ is the interestingness of the $i$-th topic for the teacher.</p><p>The third line of the input contains $n$ integers $b_1, b_2, \dots, b_n$ ($1 \le b_i \le 10^9$), where $b_i$ is the interestingness of the $i$-th topic for the students.</p>

## Output

<p>Print one integer — the number of <span class="tex-font-style-bf">good</span> pairs of topic.</p>





```input1
5
4 8 2 6 2
4 5 4 1 3
```




```input2
4
1 3 2 4
1 3 2 4
```




```output1
7
```




```output2
0
```


