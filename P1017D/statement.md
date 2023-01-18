## Description

<div><p>Childan is making up a legendary story and trying to sell his forgery&nbsp;— a necklace with a strong sense of "<span class="tex-font-style-it">Wu</span>" to the Kasouras. But Mr. Kasoura is challenging the truth of Childan's story. So he is going to ask a few questions about Childan's so-called "personal treasure" necklace.</p><p>This "personal treasure" is a multiset $S$ of $m$ "<span class="tex-font-style-it">01-strings</span>".</p><p>A "<span class="tex-font-style-it">01-string</span>" is a string that contains $n$ characters "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">1</span>". For example, if $n=4$, strings "<span class="tex-font-style-tt">0110</span>", "<span class="tex-font-style-tt">0000</span>", and "<span class="tex-font-style-tt">1110</span>" are "<span class="tex-font-style-it">01-strings</span>", but "<span class="tex-font-style-tt">00110</span>" (there are $5$ characters, not $4$) and "<span class="tex-font-style-tt">zero</span>" (unallowed characters) are not.</p><p><span class="tex-font-style-bf">Note that the multiset $S$ can contain equal elements.</span></p><p>Frequently, Mr. Kasoura will provide a "<span class="tex-font-style-it">01-string</span>" $t$ and ask Childan how many strings $s$ are in the multiset $S$ such that the "<span class="tex-font-style-it">Wu</span>" value of the pair $(s, t)$ is <span class="tex-font-style-bf">not greater</span> than $k$. </p><p>Mrs. Kasoura and Mr. Kasoura think that if $s_i = t_i$ ($1\leq i\leq n$) then the "<span class="tex-font-style-it">Wu</span>" value of the character pair equals to $w_i$, otherwise $0$. The "<span class="tex-font-style-it">Wu</span>" value of the "<span class="tex-font-style-it">01-string</span>" pair is the sum of the "<span class="tex-font-style-it">Wu</span>" values of every character pair. Note that the length of every "<span class="tex-font-style-it">01-string</span>" is equal to $n$.</p><p>For example, if $w=[4, 5, 3, 6]$, "<span class="tex-font-style-it">Wu</span>" of ("<span class="tex-font-style-tt">1001</span>", "<span class="tex-font-style-tt">1100</span>") is $7$ because these strings have equal characters only on the first and third positions, so $w_1+w_3=4+3=7$.</p><p>You need to help Childan to answer Mr. Kasoura's queries. That is to find the number of strings in the multiset $S$ such that the "<span class="tex-font-style-it">Wu</span>" value of the pair is not greater than $k$.</p></div><div class="input-specification"><p>The first line contains three integers $n$, $m$, and $q$ ($1\leq n\leq 12$, $1\leq q, m\leq 5\cdot 10^5$)&nbsp;— the length of the "<span class="tex-font-style-it">01-strings</span>", the size of the multiset $S$, and the number of queries.</p><p>The second line contains $n$ integers $w_1, w_2, \ldots, w_n$ ($0 \le w_i \le 100$)&nbsp;— the value of the $i$-th caracter.</p><p>Each of the next $m$ lines contains the "<span class="tex-font-style-it">01-string</span>" $s$ of length $n$&nbsp;— the string in the multiset $S$.</p><p>Each of the next $q$ lines contains the "<span class="tex-font-style-it">01-string</span>" $t$ of length $n$ and integer $k$ ($0\leq k\leq 100$)&nbsp;— the query.</p></div><div class="output-specification"><p>For each query, print the answer for this query.</p></div>

## Input

<p>The first line contains three integers $n$, $m$, and $q$ ($1\leq n\leq 12$, $1\leq q, m\leq 5\cdot 10^5$)&nbsp;— the length of the "<span class="tex-font-style-it">01-strings</span>", the size of the multiset $S$, and the number of queries.</p><p>The second line contains $n$ integers $w_1, w_2, \ldots, w_n$ ($0 \le w_i \le 100$)&nbsp;— the value of the $i$-th caracter.</p><p>Each of the next $m$ lines contains the "<span class="tex-font-style-it">01-string</span>" $s$ of length $n$&nbsp;— the string in the multiset $S$.</p><p>Each of the next $q$ lines contains the "<span class="tex-font-style-it">01-string</span>" $t$ of length $n$ and integer $k$ ($0\leq k\leq 100$)&nbsp;— the query.</p>

## Output

<p>For each query, print the answer for this query.</p>





```input1
2 4 5
40 20
01
01
10
11
00 20
00 40
11 20
11 40
11 60

```




```input2
1 2 4
100
0
1
0 0
0 100
1 0
1 100

```




```output1
2
4
2
3
4

```




```output2
1
2
1
2

```



## Note

<p>In the first example, we can get:</p><p>"<span class="tex-font-style-it">Wu</span>" of ("<span class="tex-font-style-tt">01</span>", "<span class="tex-font-style-tt">00</span>") is $40$.</p><p>"<span class="tex-font-style-it">Wu</span>" of ("<span class="tex-font-style-tt">10</span>", "<span class="tex-font-style-tt">00</span>") is $20$.</p><p>"<span class="tex-font-style-it">Wu</span>" of ("<span class="tex-font-style-tt">11</span>", "<span class="tex-font-style-tt">00</span>") is $0$.</p><p>"<span class="tex-font-style-it">Wu</span>" of ("<span class="tex-font-style-tt">01</span>", "<span class="tex-font-style-tt">11</span>") is $20$.</p><p>"<span class="tex-font-style-it">Wu</span>" of ("<span class="tex-font-style-tt">10</span>", "<span class="tex-font-style-tt">11</span>") is $40$.</p><p>"<span class="tex-font-style-it">Wu</span>" of ("<span class="tex-font-style-tt">11</span>", "<span class="tex-font-style-tt">11</span>") is $60$.</p><p>In the first query, pairs ("<span class="tex-font-style-tt">11</span>", "<span class="tex-font-style-tt">00</span>") and ("<span class="tex-font-style-tt">10</span>", "<span class="tex-font-style-tt">00</span>") satisfy the condition since their "<span class="tex-font-style-it">Wu</span>" is not greater than $20$.</p><p>In the second query, all strings satisfy the condition.</p><p>In the third query, pairs ("<span class="tex-font-style-tt">01</span>", "<span class="tex-font-style-tt">11</span>") and ("<span class="tex-font-style-tt">01</span>", "<span class="tex-font-style-tt">11</span>") satisfy the condition. Note that since there are two "<span class="tex-font-style-tt">01</span>" strings in the multiset, the answer is $2$, not $1$.</p><p>In the fourth query, since $k$ was increased, pair ("<span class="tex-font-style-tt">10</span>", "<span class="tex-font-style-tt">11</span>") satisfies the condition too.</p><p>In the fifth query, since $k$ was increased, pair ("<span class="tex-font-style-tt">11</span>", "<span class="tex-font-style-tt">11</span>") satisfies the condition too.</p>
