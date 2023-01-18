## Description

<div><p>There is a simple way to create hard tasks: take one simple problem as the query, and try to find an algorithm that can solve it faster than bruteforce. This kind of tasks usually appears in OI contest, and usually involves data structures.</p><p>Let's try to create a task, for example, we take the "Hamming distance problem": for two binary strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> with the same length, the Hamming distance between them is the number of positions at which the corresponding symbols are different. For example, the Hamming distance between "<span class="tex-font-style-bf">0</span>01<span class="tex-font-style-bf">1</span>1" and "<span class="tex-font-style-bf">1</span>01<span class="tex-font-style-bf">0</span>1" is 2 (the different symbols are marked with bold).</p><p>We use the Hamming distance problem as a query in the following way: you are given two strings <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> and several queries. Each query will be: what is the Hamming distance between two strings <span class="tex-span"><i>a</i><sub class="lower-index"><i>p</i><sub class="lower-index">1</sub></sub><i>a</i><sub class="lower-index"><i>p</i><sub class="lower-index">1</sub> + 1</sub>...<i>a</i><sub class="lower-index"><i>p</i><sub class="lower-index">1</sub> + <i>len</i> - 1</sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>p</i><sub class="lower-index">2</sub></sub><i>b</i><sub class="lower-index"><i>p</i><sub class="lower-index">2</sub> + 1</sub>...<i>b</i><sub class="lower-index"><i>p</i><sub class="lower-index">2</sub> + <i>len</i> - 1</sub></span>?</p><p>Note, that in this problem the strings are <span class="tex-font-style-bf">zero-based</span>, that is <span class="tex-span"><i>s</i> = <i>s</i><sub class="lower-index">0</sub><i>s</i><sub class="lower-index">1</sub>... <i>s</i><sub class="lower-index">|<i>s</i>| - 1</sub></span>.</p></div><div class="input-specification"><p>The first line contains a string <span class="tex-span"><i>a</i></span> <span class="tex-span">(1 ≤ |<i>a</i>| ≤ 200000)</span>. The second line contains a string <span class="tex-span"><i>b</i></span> <span class="tex-span">(1 ≤ |<i>b</i>| ≤ 200000)</span>. Each character of both strings is either "<span class="tex-font-style-tt">0</span>" or "<span class="tex-font-style-tt">1</span>".</p><p>The third line contains an integer <span class="tex-span"><i>q</i></span> <span class="tex-span">(1 ≤ <i>q</i> ≤ 400000)</span> — the number of queries. Each of the following <span class="tex-span"><i>q</i></span> lines contains three integers: <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>len</i></span> <span class="tex-span">(0 ≤ <i>p</i><sub class="lower-index">1</sub> ≤ |<i>a</i>| - <i>len</i>;&nbsp;0 ≤ <i>p</i><sub class="lower-index">2</sub> ≤ |<i>b</i>| - <i>len</i>)</span>, these numbers denote the parameters of the current query.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>q</i></span> integers — the answers for the queries.</p></div>

## Input

<p>The first line contains a string <span class="tex-span"><i>a</i></span> <span class="tex-span">(1 ≤ |<i>a</i>| ≤ 200000)</span>. The second line contains a string <span class="tex-span"><i>b</i></span> <span class="tex-span">(1 ≤ |<i>b</i>| ≤ 200000)</span>. Each character of both strings is either "<span class="tex-font-style-tt">0</span>" or "<span class="tex-font-style-tt">1</span>".</p><p>The third line contains an integer <span class="tex-span"><i>q</i></span> <span class="tex-span">(1 ≤ <i>q</i> ≤ 400000)</span> — the number of queries. Each of the following <span class="tex-span"><i>q</i></span> lines contains three integers: <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>len</i></span> <span class="tex-span">(0 ≤ <i>p</i><sub class="lower-index">1</sub> ≤ |<i>a</i>| - <i>len</i>;&nbsp;0 ≤ <i>p</i><sub class="lower-index">2</sub> ≤ |<i>b</i>| - <i>len</i>)</span>, these numbers denote the parameters of the current query.</p>

## Output

<p>Output <span class="tex-span"><i>q</i></span> integers — the answers for the queries.</p>





```input1
101010
11110000
3
0 0 3
2 3 4
5 7 1

```




```input2
10001010101011001010100101010011010
101010100101001010100100101010
5
0 0 12
3 9 7
6 4 15
12 15 10
13 3 20

```




```output1
1
1
0

```




```output2
5
4
3
5
13

```


