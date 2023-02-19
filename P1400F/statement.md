## Description

<div><p>You are given an integer value $x$ and a string $s$ consisting of digits from $1$ to $9$ inclusive.</p><p>A substring of a string is a contiguous subsequence of that string.</p><p>Let $f(l, r)$ be the sum of digits of a substring $s[l..r]$.</p><p>Let's call substring $s[l_1..r_1]$ <span class="tex-font-style-it">$x$-prime</span> if </p><ul> <li> $f(l_1, r_1) = x$; </li><li> there are no values $l_2, r_2$ such that <ul> <li> $l_1 \le l_2 \le r_2 \le r_1$; </li><li> $f(l_2, r_2) \neq x$; </li><li> $x$ is divisible by $f(l_2, r_2)$. </li></ul> </li></ul><p>You are allowed to erase some characters from the string. If you erase a character, the two resulting parts of the string are concatenated without changing their order.</p><p>What is the minimum number of characters you should erase from the string so that there are no <span class="tex-font-style-it">$x$-prime</span> substrings in it? If there are no <span class="tex-font-style-it">$x$-prime</span> substrings in the given string $s$, then print $0$.</p></div><div class="input-specification"><p>The first line contains a string $s$ ($1 \le |s| \le 1000$). $s$ contains only digits from $1$ to $9$ inclusive.</p><p>The second line contains an integer $x$ ($1 \le x \le 20$).</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the minimum number of characters you should erase from the string so that there are no <span class="tex-font-style-it">$x$-prime</span> substrings in it. If there are no <span class="tex-font-style-it">$x$-prime</span> substrings in the given string $s$, then print $0$.</p></div>

## Input

<p>The first line contains a string $s$ ($1 \le |s| \le 1000$). $s$ contains only digits from $1$ to $9$ inclusive.</p><p>The second line contains an integer $x$ ($1 \le x \le 20$).</p>

## Output

<p>Print a single integer&nbsp;— the minimum number of characters you should erase from the string so that there are no <span class="tex-font-style-it">$x$-prime</span> substrings in it. If there are no <span class="tex-font-style-it">$x$-prime</span> substrings in the given string $s$, then print $0$.</p>





```input1
116285317
8
```




```input2
314159265359
1
```




```input3
13
13
```




```input4
3434343434
7
```




```output1
2
```




```output2
2
```




```output3
0
```




```output4
5
```



## Note

<p>In the first example there are two $8$-prime substrings "<span class="tex-font-style-tt">8</span>" and "<span class="tex-font-style-tt">53</span>". You can erase these characters to get rid of both: "<span class="tex-font-style-tt">1162<span class="tex-font-style-underline">85</span>317</span>". The resulting string "<span class="tex-font-style-tt">1162317</span>" contains no $8$-prime substrings. Removing these characters is also a valid answer: "<span class="tex-font-style-tt">1162<span class="tex-font-style-underline">8</span>5<span class="tex-font-style-underline">3</span>17</span>".</p><p>In the second example you just have to erase both ones.</p><p>In the third example there are no $13$-prime substrings. There are no substrings with the sum of digits equal to $13$ at all.</p><p>In the fourth example you can have neither "<span class="tex-font-style-tt">34</span>", nor "<span class="tex-font-style-tt">43</span>" in a string. Thus, you have to erase either all threes or all fours. There are $5$ of each of them, so it doesn't matter which.</p>
