## Description

<div><p>Let's denote <span class="tex-font-style-it">correct match equation</span> (we will denote it as CME) an equation $a + b = c$ there all integers $a$, $b$ and $c$ are greater than zero.</p><p>For example, equations $2 + 2 = 4$ (<span class="tex-font-style-tt">||+||=||||</span>) and $1 + 2 = 3$ (<span class="tex-font-style-tt">|+||=|||</span>) are CME but equations $1 + 2 = 4$ (<span class="tex-font-style-tt">|+||=||||</span>), $2 + 2 = 3$ (<span class="tex-font-style-tt">||+||=|||</span>), and $0 + 1 = 1$ (<span class="tex-font-style-tt">+|=|</span>) are not.</p><p>Now, you have $n$ matches. You want to assemble a CME using <span class="tex-font-style-bf">all</span> your matches. Unfortunately, it is possible that you can't assemble the CME using all matches. But you can buy some extra matches and then assemble CME!</p><p>For example, if $n = 2$, you can buy two matches and assemble <span class="tex-font-style-tt">|+|=||</span>, and if $n = 5$ you can buy one match and assemble <span class="tex-font-style-tt">||+|=|||</span>. </p><center> <img class="tex-graphics" src="file://cHSO1JB2.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Calculate the minimum number of matches which you have to buy for assembling CME.</p><p>Note, that you have to answer $q$ independent queries.</p></div><div class="input-specification"><p>The first line contains one integer $q$ ($1 \le q \le 100$)&nbsp;— the number of queries.</p><p>The only line of each query contains one integer $n$ ($2 \le n \le 10^9$)&nbsp;— the number of matches.</p></div><div class="output-specification"><p>For each test case print one integer in single line&nbsp;— the minimum number of matches which you have to buy for assembling CME. </p></div>

## Input

<p>The first line contains one integer $q$ ($1 \le q \le 100$)&nbsp;— the number of queries.</p><p>The only line of each query contains one integer $n$ ($2 \le n \le 10^9$)&nbsp;— the number of matches.</p>

## Output

<p>For each test case print one integer in single line&nbsp;— the minimum number of matches which you have to buy for assembling CME. </p>





```input1
4
2
5
8
11
```




```output1
2
1
0
1
```



## Note

<p>The first and second queries are explained in the statement.</p><p>In the third query, you can assemble $1 + 3 = 4$ (<span class="tex-font-style-tt">|+|||=||||</span>) without buying matches.</p><p>In the fourth query, buy one match and assemble $2 + 4 = 6$ (<span class="tex-font-style-tt">||+||||=||||||</span>).</p>
