## Description

<div><p><span class="tex-font-style-it">DZY loves strings, and he enjoys collecting them.</span></p><p>In China, many people like to use strings containing their names' initials, for example: <span class="tex-font-style-tt">xyz</span>, <span class="tex-font-style-tt">jcvb</span>, <span class="tex-font-style-tt">dzy</span>, <span class="tex-font-style-tt">dyh</span>.</p><p>Once DZY found a lucky string <span class="tex-span"><i>s</i></span>. A lot of pairs of good friends came to DZY when they heard about the news. The first member of the <span class="tex-span"><i>i</i></span>-th pair has name <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, the second one has name <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. Each pair wondered if there is a substring of the lucky string containing both of their names. If so, they want to find the one with minimum length, which can give them good luck and make their friendship last forever.</p><p>Please help DZY for each pair find the minimum length of the substring of <span class="tex-span"><i>s</i></span> that contains both <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, or point out that such substring doesn't exist.</p><p>A substring of <span class="tex-span"><i>s</i></span> is a string <span class="tex-span"><i>s</i><sub class="lower-index"><i>l</i></sub><i>s</i><sub class="lower-index"><i>l</i> + 1</sub>... <i>s</i><sub class="lower-index"><i>r</i></sub></span> for some integers <span class="tex-span"><i>l</i>, <i>r</i></span> <span class="tex-span">(1 ≤ <i>l</i> ≤ <i>r</i> ≤ |<i>s</i>|)</span>. The length of such the substring is <span class="tex-span">(<i>r</i> - <i>l</i> + 1)</span>.</p><p>A string <span class="tex-span"><i>p</i></span> contains some another string <span class="tex-span"><i>q</i></span> if there is a substring of <span class="tex-span"><i>p</i></span> equal to <span class="tex-span"><i>q</i></span>.</p></div><div class="input-specification"><p>The first line contains a string <span class="tex-span"><i>s</i></span> <span class="tex-span">(1 ≤ |<i>s</i>| ≤ 50000)</span>.</p><p>The second line contains a non-negative integer <span class="tex-span"><i>q</i></span> <span class="tex-span">(0 ≤ <i>q</i> ≤ 100000)</span> — the number of pairs. Each of the next <span class="tex-span"><i>q</i></span> lines describes a pair, the line contains two space-separated strings <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ |<i>a</i><sub class="lower-index"><i>i</i></sub>|, |<i>b</i><sub class="lower-index"><i>i</i></sub>| ≤ 4)</span>.</p><p>It is guaranteed that all the strings only consist of lowercase English letters.</p></div><div class="output-specification"><p>For each pair, print a line containing a single integer — the minimum length of the required substring. If there is no such substring, output <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains a string <span class="tex-span"><i>s</i></span> <span class="tex-span">(1 ≤ |<i>s</i>| ≤ 50000)</span>.</p><p>The second line contains a non-negative integer <span class="tex-span"><i>q</i></span> <span class="tex-span">(0 ≤ <i>q</i> ≤ 100000)</span> — the number of pairs. Each of the next <span class="tex-span"><i>q</i></span> lines describes a pair, the line contains two space-separated strings <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ |<i>a</i><sub class="lower-index"><i>i</i></sub>|, |<i>b</i><sub class="lower-index"><i>i</i></sub>| ≤ 4)</span>.</p><p>It is guaranteed that all the strings only consist of lowercase English letters.</p>

## Output

<p>For each pair, print a line containing a single integer — the minimum length of the required substring. If there is no such substring, output <span class="tex-font-style-tt">-1</span>.</p>





```input1
xudyhduxyz
3
xyz xyz
dyh xyz
dzy xyz

```




```input2
abcabd
3
a c
ab abc
ab d

```




```input3
baabcabaaa
2
abca baa
aa aba

```




```output1
3
8
-1

```




```output2
2
3
3

```




```output3
6
4

```



## Note

<p>The shortest substrings in the first sample are: <span class="tex-font-style-tt">xyz</span>, <span class="tex-font-style-tt">dyhduxyz</span>.</p><p>The shortest substrings in the second sample are: <span class="tex-font-style-tt">ca</span>, <span class="tex-font-style-tt">abc</span> and <span class="tex-font-style-tt">abd</span>.</p><p>The shortest substrings in the third sample are: <span class="tex-font-style-tt">baabca</span> and <span class="tex-font-style-tt">abaa</span>.</p>
