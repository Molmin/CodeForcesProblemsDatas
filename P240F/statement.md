## Description

<div><p>A boy named Leo doesn't miss a single TorCoder contest round. On the last TorCoder round number 100666 Leo stumbled over the following problem. He was given a string <span class="tex-span"><i>s</i></span>, consisting of <span class="tex-span"><i>n</i></span> lowercase English letters, and <span class="tex-span"><i>m</i></span> queries. Each query is characterised by a pair of integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>. </p><p>We'll consider the letters in the string numbered from 1 to <span class="tex-span"><i>n</i></span> from left to right, that is, <span class="tex-span"><i>s</i> = <i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index"><i>n</i></sub></span>. </p><p>After each query he must swap letters with indexes from <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> inclusive in string <span class="tex-span"><i>s</i></span> so as to make substring <span class="tex-span">(<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>)</span> a palindrome. If there are multiple such letter permutations, you should choose the one where string <span class="tex-span">(<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>)</span> will be lexicographically minimum. If no such permutation exists, you should ignore the query (that is, not change string <span class="tex-span"><i>s</i></span>).</p><p>Everybody knows that on TorCoder rounds input line and array size limits never exceed <span class="tex-span">60</span>, so Leo solved this problem easily. Your task is to solve the problem on a little bit larger limits. Given string <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>m</i></span> queries, print the string that results after applying all <span class="tex-span"><i>m</i></span> queries to string <span class="tex-span"><i>s</i></span>.</p></div><div class="input-specification"><p>The first input line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the string length and the number of the queries.</p><p>The second line contains string <span class="tex-span"><i>s</i></span>, consisting of <span class="tex-span"><i>n</i></span> lowercase Latin letters.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains a pair of integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — a query to apply to the string. </p></div><div class="output-specification"><p>In a single line print the result of applying <span class="tex-span"><i>m</i></span> queries to string <span class="tex-span"><i>s</i></span>. Print the queries in the order in which they are given in the input.</p></div>

## Input

<p>The first input line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the string length and the number of the queries.</p><p>The second line contains string <span class="tex-span"><i>s</i></span>, consisting of <span class="tex-span"><i>n</i></span> lowercase Latin letters.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains a pair of integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — a query to apply to the string. </p>

## Output

<p>In a single line print the result of applying <span class="tex-span"><i>m</i></span> queries to string <span class="tex-span"><i>s</i></span>. Print the queries in the order in which they are given in the input.</p>





```input1
7 2
aabcbaa
1 3
5 7

```




```input2
3 2
abc
1 2
2 3

```




```output1
abacaba

```




```output2
abc

```



## Note

<p>A <span class="tex-font-style-it">substring</span> <span class="tex-span">(<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>)</span> <span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> of string <span class="tex-span"><i>s</i> = <i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index"><i>n</i></sub></span> of length <span class="tex-span"><i>n</i></span> is a sequence of characters <span class="tex-span"><i>s</i><sub class="lower-index"><i>l</i><sub class="lower-index"><i>i</i></sub></sub><i>s</i><sub class="lower-index"><i>l</i><sub class="lower-index"><i>i</i> + 1</sub></sub>...<i>s</i><sub class="lower-index"><i>r</i><sub class="lower-index"><i>i</i></sub></sub></span>.</p><p>A string is a <span class="tex-font-style-it">palindrome</span>, if it reads the same from left to right and from right to left.</p><p>String <span class="tex-span"><i>x</i><sub class="lower-index">1</sub><i>x</i><sub class="lower-index">2</sub>... <i>x</i><sub class="lower-index"><i>p</i></sub></span> is <span class="tex-font-style-it">lexicographically smaller</span> than string <span class="tex-span"><i>y</i><sub class="lower-index">1</sub><i>y</i><sub class="lower-index">2</sub>... <i>y</i><sub class="lower-index"><i>q</i></sub></span>, if either <span class="tex-span"><i>p</i> &lt; <i>q</i></span> and <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub> = <i>y</i><sub class="lower-index">2</sub>, ... , <i>x</i><sub class="lower-index"><i>p</i></sub> = <i>y</i><sub class="lower-index"><i>p</i></sub></span>, or exists such number <span class="tex-span"><i>r</i></span> <span class="tex-span">(<i>r</i> &lt; <i>p</i>, <i>r</i> &lt; <i>q</i>)</span>, that <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub> = <i>y</i><sub class="lower-index">2</sub>, ... , <i>x</i><sub class="lower-index"><i>r</i></sub> = <i>y</i><sub class="lower-index"><i>r</i></sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index"><i>r</i> + 1</sub> &lt; <i>y</i><sub class="lower-index"><i>r</i> + 1</sub></span>.</p>
