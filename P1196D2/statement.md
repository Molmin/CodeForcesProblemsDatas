## Description

<div><p><span class="tex-font-style-bf">The only difference between easy and hard versions is the size of the input</span>.</p><p>You are given a string $s$ consisting of $n$ characters, each character is '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">G</span>' or '<span class="tex-font-style-tt">B</span>'.</p><p>You are also given an integer $k$. Your task is to change the minimum number of characters in the initial string $s$ so that after the changes there will be a string of length $k$ that is a substring of $s$, and is also a substring of the infinite string "<span class="tex-font-style-tt">RGBRGBRGB ...</span>".</p><p>A string $a$ is a substring of string $b$ if there exists a positive integer $i$ such that $a_1 = b_i$, $a_2 = b_{i + 1}$, $a_3 = b_{i + 2}$, ..., $a_{|a|} = b_{i + |a| - 1}$. For example, strings "<span class="tex-font-style-tt">GBRG</span>", "<span class="tex-font-style-tt">B</span>", "<span class="tex-font-style-tt">BR</span>" are substrings of the infinite string "<span class="tex-font-style-tt">RGBRGBRGB ...</span>" while "<span class="tex-font-style-tt">GR</span>", "<span class="tex-font-style-tt">RGR</span>" and "<span class="tex-font-style-tt">GGG</span>" are not.</p><p>You have to answer $q$ independent queries.</p></div><div class="input-specification"><p>The first line of the input contains one integer $q$ ($1 \le q \le 2 \cdot 10^5$)&nbsp;— the number of queries. Then $q$ queries follow.</p><p>The first line of the query contains two integers $n$ and $k$ ($1 \le k \le n \le 2 \cdot 10^5$)&nbsp;— the length of the string $s$ and the length of the substring.</p><p>The second line of the query contains a string $s$ consisting of $n$ characters '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">G</span>' and '<span class="tex-font-style-tt">B</span>'.</p><p>It is guaranteed that the sum of $n$ over all queries does not exceed $2 \cdot 10^5$ ($\sum n \le 2 \cdot 10^5$).</p></div><div class="output-specification"><p>For each query print one integer&nbsp;— the minimum number of characters you need to change in the initial string $s$ so that after changing there will be a substring of length $k$ in $s$ that is also a substring of the infinite string "<span class="tex-font-style-tt">RGBRGBRGB ...</span>".</p></div>

## Input

<p>The first line of the input contains one integer $q$ ($1 \le q \le 2 \cdot 10^5$)&nbsp;— the number of queries. Then $q$ queries follow.</p><p>The first line of the query contains two integers $n$ and $k$ ($1 \le k \le n \le 2 \cdot 10^5$)&nbsp;— the length of the string $s$ and the length of the substring.</p><p>The second line of the query contains a string $s$ consisting of $n$ characters '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">G</span>' and '<span class="tex-font-style-tt">B</span>'.</p><p>It is guaranteed that the sum of $n$ over all queries does not exceed $2 \cdot 10^5$ ($\sum n \le 2 \cdot 10^5$).</p>

## Output

<p>For each query print one integer&nbsp;— the minimum number of characters you need to change in the initial string $s$ so that after changing there will be a substring of length $k$ in $s$ that is also a substring of the infinite string "<span class="tex-font-style-tt">RGBRGBRGB ...</span>".</p>





```input1
3
5 2
BGGGG
5 3
RBRGR
5 5
BBBRR
```




```output1
1
0
3
```



## Note

<p>In the first example, you can change the first character to '<span class="tex-font-style-tt">R</span>' and obtain the substring "<span class="tex-font-style-tt">RG</span>", or change the second character to '<span class="tex-font-style-tt">R</span>' and obtain "<span class="tex-font-style-tt">BR</span>", or change the third, fourth or fifth character to '<span class="tex-font-style-tt">B</span>' and obtain "<span class="tex-font-style-tt">GB</span>".</p><p>In the second example, the substring is "<span class="tex-font-style-tt">BRG</span>".</p>
