## Description

<div><p>Let's say that two strings $s$ and $t$ <span class="tex-font-style-it">rhyme</span> if both strings have length at least $k$, and their last $k$ characters are equal. For example, if $k = 3$, the strings <span class="tex-font-style-tt">abcd</span> and <span class="tex-font-style-tt">cebcd</span> rhyme, the strings <span class="tex-font-style-tt">ab</span> and <span class="tex-font-style-tt">ab</span> don't rhyme, the strings <span class="tex-font-style-tt">aaaa</span> and <span class="tex-font-style-tt">aaaaa</span> rhyme, the strings <span class="tex-font-style-tt">abcd</span> and <span class="tex-font-style-tt">abce</span> don't rhyme.</p><p>You have $n$ pairs of strings $(s_i, t_i)$, and for each pair of strings you know, should they rhyme or should not.</p><p>Find all possible non-negative integer values for $k$ such that pairs that have to rhyme, rhyme and pairs that must not rhyme, don't rhyme.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;— the number of string pairs.</p><p>Next $n$ lines contains descriptions of pairs&nbsp;— one per line. The $i$-th line contains space-separated strings $s_i$ and $t_i$ and marker $r_i$. Strings are non-empty, consist of lowercase Latin letters and each have length at most $2 \cdot 10^5$. The marker $r_i$ equals to $1$ if strings have to rhyme, or $0$ if they must not rhyme.</p><p>It's guaranteed that for each test case there is at least one pair with $r_i$ equal to $1$ and that the total length of all strings over all test cases doesn't exceed $4 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, firstly print integer $m$&nbsp;— the number of possible non-negative integer values of $k$ such that pairs that have to rhyme, rhyme and pairs that must not rhyme, don't rhyme. Next, print all these values of $k$ (without repetitions). You can print them in any order.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;— the number of string pairs.</p><p>Next $n$ lines contains descriptions of pairs&nbsp;— one per line. The $i$-th line contains space-separated strings $s_i$ and $t_i$ and marker $r_i$. Strings are non-empty, consist of lowercase Latin letters and each have length at most $2 \cdot 10^5$. The marker $r_i$ equals to $1$ if strings have to rhyme, or $0$ if they must not rhyme.</p><p>It's guaranteed that for each test case there is at least one pair with $r_i$ equal to $1$ and that the total length of all strings over all test cases doesn't exceed $4 \cdot 10^5$.</p>

## Output

<p>For each test case, firstly print integer $m$&nbsp;— the number of possible non-negative integer values of $k$ such that pairs that have to rhyme, rhyme and pairs that must not rhyme, don't rhyme. Next, print all these values of $k$ (without repetitions). You can print them in any order.</p>





```input1
3
1
kotlin heroes 1
2
join kotlin 1
episode eight 0
4
abc abcdef 0
xyz zzz 1
aaa bba 0
c d 0
```




```output1
1
0
2
1 2
0
```



## Note

<p>In the first test case, if $k$ is at least $1$ then <span class="tex-font-style-tt">kotli<span class="tex-font-style-underline">n</span></span> and <span class="tex-font-style-tt">heroe<span class="tex-font-style-underline">s</span></span> don't rhyme.</p><p>In the second test case, for $k = 2$ <span class="tex-font-style-tt">jo<span class="tex-font-style-underline">in</span></span> and <span class="tex-font-style-tt">kotl<span class="tex-font-style-underline">in</span></span> rhyme, and <span class="tex-font-style-tt">episo<span class="tex-font-style-underline">de</span></span> and <span class="tex-font-style-tt">eig<span class="tex-font-style-underline">ht</span></span> don't rhyme.</p>
