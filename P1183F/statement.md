## Description

<div><p>One important contest will take place on the most famous programming platform (Topforces) very soon!</p><p>The authors have a pool of $n$ problems and should choose <span class="tex-font-style-bf">at most three</span> of them into this contest. The prettiness of the $i$-th problem is $a_i$. The authors have to compose the most pretty contest (in other words, the cumulative prettinesses of chosen problems should be <span class="tex-font-style-bf">maximum possible</span>).</p><p>But there is one important thing in the contest preparation: because of some superstitions of authors, the prettinesses of problems cannot divide each other. In other words, if the prettinesses of chosen problems are $x, y, z$, then $x$ should be divisible by neither $y$, nor $z$, $y$ should be divisible by neither $x$, nor $z$ and $z$ should be divisible by neither $x$, nor $y$. If the prettinesses of chosen problems are $x$ and $y$ then neither $x$ should be divisible by $y$ nor $y$ should be divisible by $x$. Any contest composed from one problem is considered good.</p><p>Your task is to find out the maximum possible total prettiness of the contest composed of <span class="tex-font-style-bf">at most three</span> problems from the given pool.</p><p>You have to answer $q$ independent queries.</p><p><span class="tex-font-style-bf">If you are Python programmer, consider using PyPy instead of Python when you submit your code.</span></p></div><div class="input-specification"><p>The first line of the input contains one integer $q$ ($1 \le q \le 2 \cdot 10^5$) — the number of queries.</p><p>The first line of the query contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of problems.</p><p>The second line of the query contains $n$ integers $a_1, a_2, \dots, a_n$ ($2 \le a_i \le 2 \cdot 10^5$), where $a_i$ is the prettiness of the $i$-th problem.</p><p>It is guaranteed that the sum of $n$ over all queries does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each query print one integer — the maximum possible cumulative prettiness of the contest composed of <span class="tex-font-style-bf">at most three</span> problems from the given pool of problems in the query.</p></div>

## Input

<p>The first line of the input contains one integer $q$ ($1 \le q \le 2 \cdot 10^5$) — the number of queries.</p><p>The first line of the query contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of problems.</p><p>The second line of the query contains $n$ integers $a_1, a_2, \dots, a_n$ ($2 \le a_i \le 2 \cdot 10^5$), where $a_i$ is the prettiness of the $i$-th problem.</p><p>It is guaranteed that the sum of $n$ over all queries does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each query print one integer — the maximum possible cumulative prettiness of the contest composed of <span class="tex-font-style-bf">at most three</span> problems from the given pool of problems in the query.</p>





```input1
3
4
5 6 15 30
4
10 6 30 15
3
3 4 6
```




```output1
30
31
10
```


