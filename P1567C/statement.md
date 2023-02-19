## Description

<div><p>Alice has just learned addition. However, she hasn't learned the concept of "carrying" fully&nbsp;— instead of carrying to the <span class="tex-font-style-it">next</span> column, she carries to the column <span class="tex-font-style-it">two columns to the left</span>.</p><p>For example, the <span class="tex-font-style-bf">regular</span> way to evaluate the sum $2039 + 2976$ would be as shown: </p><center> <img class="tex-graphics" src="file://ToavdG7w.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>However, Alice evaluates it as shown: </p><center> <img class="tex-graphics" src="file://rBKYtl4m.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In particular, this is what she does: </p><ul> <li> add $9$ and $6$ to make $15$, and carry the $1$ to the column <span class="tex-font-style-it">two columns to the left</span>, i.&nbsp;e. to the column "$0$ $9$"; </li><li> add $3$ and $7$ to make $10$ and carry the $1$ to the column <span class="tex-font-style-it">two columns to the left</span>, i.&nbsp;e. to the column "$2$ $2$"; </li><li> add $1$, $0$, and $9$ to make $10$ and carry the $1$ to the column <span class="tex-font-style-it">two columns to the left</span>, i.&nbsp;e. to the column above the plus sign; </li><li> add $1$, $2$ and $2$ to make $5$; </li><li> add $1$ to make $1$. </li></ul> Thus, she ends up with the incorrect result of $15005$.<p>Alice comes up to Bob and says that she has added two numbers to get a result of $n$. However, Bob knows that Alice adds in her own way. Help Bob find the number of <span class="tex-font-style-it">ordered pairs of positive integers</span> such that when Alice adds them, she will get a result of $n$. Note that pairs $(a, b)$ and $(b, a)$ are considered different if $a \ne b$.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The only line of each test case contains an integer $n$ ($2 \leq n \leq 10^9$)&nbsp;— the number Alice shows Bob.</p></div><div class="output-specification"><p>For each test case, output one integer&nbsp;— the number of <span class="tex-font-style-it">ordered</span> pairs of <span class="tex-font-style-bf">positive integers</span> such that when Alice adds them, she will get a result of $n$. </p></div>

## Input

<p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The only line of each test case contains an integer $n$ ($2 \leq n \leq 10^9$)&nbsp;— the number Alice shows Bob.</p>

## Output

<p>For each test case, output one integer&nbsp;— the number of <span class="tex-font-style-it">ordered</span> pairs of <span class="tex-font-style-bf">positive integers</span> such that when Alice adds them, she will get a result of $n$. </p>





```input1
5
100
12
8
2021
10000
```




```output1
9
4
7
44
99
```



## Note

<p>In the first test case, when Alice evaluates any of the sums $1 + 9$, $2 + 8$, $3 + 7$, $4 + 6$, $5 + 5$, $6 + 4$, $7 + 3$, $8 + 2$, or $9 + 1$, she will get a result of $100$. The picture below shows how Alice evaluates $6 + 4$: </p><center> <img class="tex-graphics" src="file://J2jTEDtZ.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
