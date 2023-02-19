## Description

<div><p>Boboniu defines <span class="tex-font-style-it">BN-string</span> as a string $s$ of characters 'B' and 'N'.</p><p>You can perform the following operations on the BN-string $s$:</p><ul> <li> Remove a character of $s$. </li><li> Remove a substring "<span class="tex-font-style-tt">BN</span>" or "<span class="tex-font-style-tt">NB</span>" of $s$. </li><li> Add a character 'B' or 'N' to the end of $s$. </li><li> Add a string "<span class="tex-font-style-tt">BN</span>" or "<span class="tex-font-style-tt">NB</span>" to the end of $s$. </li></ul><p>Note that a string $a$ is a <span class="tex-font-style-it">substring</span> of a string $b$ if $a$ can be obtained from $b$ by deletion of several (possibly, zero or all) characters from the beginning and several (possibly, zero or all) characters from the end.</p><p>Boboniu thinks that BN-strings $s$ and $t$ are <span class="tex-font-style-it">similar</span> if and only if:</p><ul> <li> $|s|=|t|$. </li><li> There exists a permutation $p_1, p_2, \ldots, p_{|s|}$ such that for all $i$ ($1\le i\le |s|$), $s_{p_i}=t_i$. </li></ul><p>Boboniu also defines $\text{dist}(s,t)$, the <span class="tex-font-style-it">distance</span> between $s$ and $t$, as the minimum number of operations that makes $s$ <span class="tex-font-style-it">similar</span> to $t$.</p><p>Now Boboniu gives you $n$ non-empty BN-strings $s_1,s_2,\ldots, s_n$ and asks you to find a <span class="tex-font-style-bf">non-empty</span> BN-string $t$ such that the maximum distance to string $s$ is minimized, i.e. you need to minimize $\max_{i=1}^n \text{dist}(s_i,t)$.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1\le n\le 3\cdot 10^5$).</p><p>Each of the next $n$ lines contains a string $s_i$ ($1\le |s_i| \le 5\cdot 10^5$). It is guaranteed that $s_i$ only contains 'B' and 'N'. The sum of $|s_i|$ does not exceed $5\cdot 10^5$.</p></div><div class="output-specification"><p>In the first line, print the minimum $\max_{i=1}^n \text{dist}(s_i,t)$.</p><p>In the second line, print the suitable $t$.</p><p>If there are several possible $t$'s, you can print any.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1\le n\le 3\cdot 10^5$).</p><p>Each of the next $n$ lines contains a string $s_i$ ($1\le |s_i| \le 5\cdot 10^5$). It is guaranteed that $s_i$ only contains 'B' and 'N'. The sum of $|s_i|$ does not exceed $5\cdot 10^5$.</p>

## Output

<p>In the first line, print the minimum $\max_{i=1}^n \text{dist}(s_i,t)$.</p><p>In the second line, print the suitable $t$.</p><p>If there are several possible $t$'s, you can print any.</p>





```input1
3
B
N
BN
```




```input2
10
N
BBBBBB
BNNNBBNBB
NNNNBNBNNBNNNBBN
NBNBN
NNNNNN
BNBNBNBBBBNNNNBBBBNNBBNBNBBNBBBBBBBB
NNNNBN
NBBBBBBBB
NNNNNN
```




```input3
8
NNN
NNN
BBNNBBBN
NNNBNN
B
NNN
NNNNBNN
NNNNNNNNNNNNNNNBNNNNNNNBNB
```




```input4
3
BNNNBNNNNBNBBNNNBBNNNNBBBBNNBBBBBBNBBBBBNBBBNNBBBNBNBBBN
BBBNBBBBNNNNNBBNBBBNNNBB
BBBBBBBBBBBBBBNBBBBBNBBBBBNBBBBNB
```




```output1
1
BN
```




```output2
12
BBBBBBBBBBBBNNNNNNNNNNNN
```




```output3
12
BBBBNNNNNNNNNNNN
```




```output4
12
BBBBBBBBBBBBBBBBBBBBBBBBBBNNNNNNNNNNNN
```



## Note

<p>In the first example $\text{dist(B,BN)}=\text{dist(N,BN)}=1$, $\text{dist(BN,BN)}=0$. So the maximum distance is $1$.</p>
