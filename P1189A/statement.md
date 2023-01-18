## Description

<div><p>After playing Neo in the legendary "<span class="tex-font-style-tt">Matrix</span>" trilogy, Keanu Reeves started doubting himself: maybe we really live in virtual reality? To find if this is true, he needs to solve the following problem.</p><p>Let's call a string consisting of only zeroes and ones <span class="tex-font-style-bf">good</span> if it contains <span class="tex-font-style-bf">different</span> numbers of zeroes and ones. For example, <span class="tex-font-style-tt">1</span>, <span class="tex-font-style-tt">101</span>, <span class="tex-font-style-tt">0000</span> are good, while <span class="tex-font-style-tt">01</span>, <span class="tex-font-style-tt">1001</span>, and <span class="tex-font-style-tt">111000</span> are not good.</p><p>We are given a string $s$ of length $n$ consisting of only zeroes and ones. We need to cut $s$ into <span class="tex-font-style-bf">minimal possible</span> number of substrings $s_1, s_2, \ldots, s_k$ such that <span class="tex-font-style-bf">all</span> of them are good. More formally, we have to find <span class="tex-font-style-bf">minimal</span> by number of strings sequence of good strings $s_1, s_2, \ldots, s_k$ such that their concatenation (joining) equals $s$, i.e. $s_1 + s_2 + \dots + s_k = s$.</p><p>For example, cuttings <span class="tex-font-style-tt">110010</span> into <span class="tex-font-style-tt">110</span> and <span class="tex-font-style-tt">010</span> or into <span class="tex-font-style-tt">11</span> and <span class="tex-font-style-tt">0010</span> are valid, as <span class="tex-font-style-tt">110</span>, <span class="tex-font-style-tt">010</span>, <span class="tex-font-style-tt">11</span>, <span class="tex-font-style-tt">0010</span> are all good, and we can't cut <span class="tex-font-style-tt">110010</span> to the smaller number of substrings as <span class="tex-font-style-tt">110010</span> isn't good itself. At the same time, cutting of <span class="tex-font-style-tt">110010</span> into <span class="tex-font-style-tt">1100</span> and <span class="tex-font-style-tt">10</span> isn't valid as both strings aren't good. Also, cutting of <span class="tex-font-style-tt">110010</span> into <span class="tex-font-style-tt">1</span>, <span class="tex-font-style-tt">1</span>, <span class="tex-font-style-tt">0010</span> isn't valid, as it isn't minimal, even though all $3$ strings are good.</p><p>Can you help Keanu? We can show that the solution always exists. If there are multiple optimal answers, print any.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $n$ ($1\le n \le 100$)&nbsp;— the length of the string $s$.</p><p>The second line contains the string $s$ of length $n$ consisting only from zeros and ones.</p></div><div class="output-specification"><p>In the first line, output a single integer $k$ ($1\le k$)&nbsp;— a <span class="tex-font-style-bf">minimal</span> number of strings you have cut $s$ into.</p><p>In the second line, output $k$ strings $s_1, s_2, \ldots, s_k$ separated with spaces. The length of each string has to be positive. Their concatenation has to be equal to $s$ and all of them have to be good.</p><p>If there are multiple answers, print any.</p></div>

## Input

<p>The first line of the input contains a single integer $n$ ($1\le n \le 100$)&nbsp;— the length of the string $s$.</p><p>The second line contains the string $s$ of length $n$ consisting only from zeros and ones.</p>

## Output

<p>In the first line, output a single integer $k$ ($1\le k$)&nbsp;— a <span class="tex-font-style-bf">minimal</span> number of strings you have cut $s$ into.</p><p>In the second line, output $k$ strings $s_1, s_2, \ldots, s_k$ separated with spaces. The length of each string has to be positive. Their concatenation has to be equal to $s$ and all of them have to be good.</p><p>If there are multiple answers, print any.</p>





```input1
1
1
```




```input2
2
10
```




```input3
6
100011
```




```output1
1
1
```




```output2
2
1 0
```




```output3
2
100 011
```



## Note

<p>In the first example, the string <span class="tex-font-style-tt">1</span> wasn't cut at all. As it is good, the condition is satisfied.</p><p>In the second example, <span class="tex-font-style-tt">1</span> and <span class="tex-font-style-tt">0</span> both are good. As <span class="tex-font-style-tt">10</span> isn't good, the answer is indeed minimal.</p><p>In the third example, <span class="tex-font-style-tt">100</span> and <span class="tex-font-style-tt">011</span> both are good. As <span class="tex-font-style-tt">100011</span> isn't good, the answer is indeed minimal.</p>
