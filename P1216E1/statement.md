## Description

<div><p><span class="tex-font-style-bf">The only difference between the easy and the hard versions is the maximum value of $k$</span>.</p><p>You are given an <span class="tex-font-style-it">infinite</span> sequence of form "<span class="tex-font-style-tt">112123123412345$\dots$</span>" which consist of blocks of all consecutive positive integers written one after another. The first block consists of all numbers from $1$ to $1$, the second one — from $1$ to $2$, the third one — from $1$ to $3$, $\dots$, the $i$-th block consists of all numbers from $1$ to $i$. </p><p>So the first $56$ elements of the sequence are "<span class="tex-font-style-tt">11212312341234512345612345671234567812345678912345678910</span>". Elements of the sequence are numbered from one. For example, the $1$-st element of the sequence is $1$, the $3$-rd element of the sequence is $2$, the $20$-th element of the sequence is $5$, the $38$-th element is $2$, the $56$-th element of the sequence is $0$.</p><p>Your task is to answer $q$ independent queries. In the $i$-th query you are given one integer $k_i$. Calculate the digit at the position $k_i$ of the sequence.</p></div><div class="input-specification"><p>The first line of the input contains one integer $q$ ($1 \le q \le 500$) — the number of queries.</p><p>The $i$-th of the following $q$ lines contains one integer $k_i$ $(1 \le k_i \le 10^9)$ — the description of the corresponding query.</p></div><div class="output-specification"><p>Print $q$ lines. In the $i$-th line print one digit $x_i$ $(0 \le x_i \le 9)$ — the answer to the query $i$, i.e. $x_i$ should be equal to the element at the position $k_i$ of the sequence.</p></div>

## Input

<p>The first line of the input contains one integer $q$ ($1 \le q \le 500$) — the number of queries.</p><p>The $i$-th of the following $q$ lines contains one integer $k_i$ $(1 \le k_i \le 10^9)$ — the description of the corresponding query.</p>

## Output

<p>Print $q$ lines. In the $i$-th line print one digit $x_i$ $(0 \le x_i \le 9)$ — the answer to the query $i$, i.e. $x_i$ should be equal to the element at the position $k_i$ of the sequence.</p>





```input1
5
1
3
20
38
56
```




```input2
4
2132
506
999999999
1000000000
```




```output1
1
2
5
2
0
```




```output2
8
2
9
8
```



## Note

<p>Answers on queries from the first example are described in the problem statement.</p>
