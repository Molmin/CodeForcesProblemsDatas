## Description

<div><p>Petya once wrote a sad love song and shared it to Vasya. The song is a string consisting of lowercase English letters. Vasya made up $q$ questions about this song. Each question is about a subsegment of the song starting from the $l$-th letter to the $r$-th letter. Vasya considers a substring made up from characters on this segment and repeats each letter in the subsegment $k$ times, where $k$ is the index of the corresponding letter in the alphabet. For example, if the question is about the substring "<span class="tex-font-style-tt">abbcb</span>", then Vasya repeats letter '<span class="tex-font-style-tt">a</span>' once, each of the letters '<span class="tex-font-style-tt">b</span>' twice, letter '<span class="tex-font-style-tt">c</span>" three times, so that the resulting string is "<span class="tex-font-style-tt">abbbbcccbb</span>", its length is $10$. Vasya is interested about the length of the resulting string.</p><p>Help Petya find the length of each string obtained by Vasya.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ ($1\leq n\leq 100\,000$, $1\leq q \leq 100\,000$)&nbsp;— the length of the song and the number of questions. </p><p>The second line contains one string $s$&nbsp;— the song, consisting of $n$ lowercase letters of English letters.</p><p>Vasya's questions are contained in the next $q$ lines. Each line contains two integers $l$ and $r$ ($1 \leq l \leq r \leq n$)&nbsp;— the bounds of the question.</p></div><div class="output-specification"><p>Print $q$ lines: for each question print the length of the string obtained by Vasya.</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ ($1\leq n\leq 100\,000$, $1\leq q \leq 100\,000$)&nbsp;— the length of the song and the number of questions. </p><p>The second line contains one string $s$&nbsp;— the song, consisting of $n$ lowercase letters of English letters.</p><p>Vasya's questions are contained in the next $q$ lines. Each line contains two integers $l$ and $r$ ($1 \leq l \leq r \leq n$)&nbsp;— the bounds of the question.</p>

## Output

<p>Print $q$ lines: for each question print the length of the string obtained by Vasya.</p>





```input1
7 3
abacaba
1 3
2 5
1 7
```




```input2
7 4
abbabaa
1 3
5 7
6 6
2 4
```




```input3
13 7
sonoshikumiwo
1 5
2 10
7 7
1 13
4 8
2 5
3 9
```




```output1
4
7
11
```




```output2
5
4
1
5
```




```output3
82
125
9
191
62
63
97
```



## Note

<p>In the first example Vasya is interested in three questions. In the first question Vasya considers the substring "<span class="tex-font-style-tt">aba</span>", that transforms to "<span class="tex-font-style-tt">abba</span>", so the answer is equal to $4$. In the second question Vasya considers "<span class="tex-font-style-tt">baca</span>", that transforms to "<span class="tex-font-style-tt">bbaccca</span>", so the answer is $7$. In the third question Vasya considers the string "<span class="tex-font-style-tt">abacaba</span>",that transforms to "<span class="tex-font-style-tt">abbacccabba</span>" of length $11$.</p>
