## Description

<div><p>You are given a string $s$, consisting of lowercase Latin letters. Every letter appears in it no more than twice.</p><p>Your task is to rearrange the letters in the string in such a way that for each pair of letters that appear exactly twice, the distance between the letters in the pair is the same. You are not allowed to add or remove letters.</p><p>It can be shown that the answer always exists. If there are multiple answers, print any of them.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^3$)&nbsp;— the number of testcases.</p><p>Each testcase consists of a non-empty string $s$, consisting of lowercase Latin letters. Every letter appears in the string no more than twice. The length of the string doesn't exceed $52$.</p></div><div class="output-specification"><p>For each testcase, print a single string. Every letter should appear in it the same number of times as it appears in string $s$. For each pair of letters that appear exactly twice, the distance between the letters in the pair should be the same.</p><p>If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^3$)&nbsp;— the number of testcases.</p><p>Each testcase consists of a non-empty string $s$, consisting of lowercase Latin letters. Every letter appears in the string no more than twice. The length of the string doesn't exceed $52$.</p>

## Output

<p>For each testcase, print a single string. Every letter should appear in it the same number of times as it appears in string $s$. For each pair of letters that appear exactly twice, the distance between the letters in the pair should be the same.</p><p>If there are multiple answers, print any of them.</p>





```input1
3
oelhl
abcdcba
ac
```




```output1
hello
ababcdc
ac
```



## Note

<p>In the first testcase of the example, the only letter that appears exactly twice is letter 'l'. You can rearrange the letters arbitrarily, since there are no distances to compare.</p><p>In the second testcase of the example, the letters that appear exactly twice are 'a', 'b' and 'c'. Initially, letters 'a' are distance $6$ apart, letters 'b' are distance $4$ apart and letters 'c' are distance $2$ apart. They are not the same, so we have to rearrange the letters. After rearrangement, letters 'a' are distance $2$ apart, letters 'b' are distance $2$ apart and letters 'c' are distance $2$ apart. They are all the same, so the answer is valid.</p><p>In the third testcase of the example, there are no letters that appear exactly twice. Thus, any rearrangement is valid. Including not changing the string at all.</p>
