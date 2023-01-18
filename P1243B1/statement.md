## Description

<div><p><span class="tex-font-style-it">This problem is different from the hard version. In this version Ujan makes <span class="tex-font-style-bf">exactly</span> one exchange. You can hack this problem only if you solve both problems.</span></p><p>After struggling and failing many times, Ujan decided to try to clean up his house again. He decided to get his strings in order first.</p><p>Ujan has two <span class="tex-font-style-bf">distinct</span> strings $s$ and $t$ of length $n$ consisting of only of lowercase English characters. He wants to make them equal. Since Ujan is lazy, he will perform the following operation exactly once: he takes two positions $i$ and $j$ ($1 \le i,j \le n$, the values $i$ and $j$ can be equal or different), and swaps the characters $s_i$ and $t_j$. Can he succeed?</p><p>Note that he has to perform this operation <span class="tex-font-style-bf">exactly</span> once. He <span class="tex-font-style-bf">has</span> to perform this operation.</p></div><div class="input-specification"><p>The first line contains a single integer $k$ ($1 \leq k \leq 10$), the number of test cases.</p><p>For each of the test cases, the first line contains a single integer $n$ ($2 \leq n \leq 10^4$), the length of the strings $s$ and $t$. </p><p>Each of the next two lines contains the strings $s$ and $t$, each having length exactly $n$. The strings consist only of lowercase English letters. It is guaranteed that strings are different.</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">Yes</span>" if Ujan can make the two strings equal and "<span class="tex-font-style-tt">No</span>" otherwise.</p><p>You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The first line contains a single integer $k$ ($1 \leq k \leq 10$), the number of test cases.</p><p>For each of the test cases, the first line contains a single integer $n$ ($2 \leq n \leq 10^4$), the length of the strings $s$ and $t$. </p><p>Each of the next two lines contains the strings $s$ and $t$, each having length exactly $n$. The strings consist only of lowercase English letters. It is guaranteed that strings are different.</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">Yes</span>" if Ujan can make the two strings equal and "<span class="tex-font-style-tt">No</span>" otherwise.</p><p>You can print each letter in any case (upper or lower).</p>





```input1
4
5
souse
houhe
3
cat
dog
2
aa
az
3
abc
bca
```




```output1
Yes
No
No
No
```



## Note

<p>In the first test case, Ujan can swap characters $s_1$ and $t_4$, obtaining the word "<span class="tex-font-style-tt">house</span>".</p><p>In the second test case, it is not possible to make the strings equal using exactly one swap of $s_i$ and $t_j$.</p>
