## Description

<div><p>Tavas lives in Tavaspolis. Tavaspolis has <span class="tex-span"><i>n</i></span> cities numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> connected by <span class="tex-span"><i>n</i> - 1</span> bidirectional roads. There exists a path between any two cities. Also each road has a length.</p><center> <img class="tex-graphics" src="file://xA6uAiTg.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Tavas' favorite strings are binary strings (they contain only 0 and 1). For any binary string like <span class="tex-span"><i>s</i> = <i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index"><i>k</i></sub></span>, <span class="tex-span"><i>T</i>(<i>s</i>)</span> is its <span class="tex-span"><i>Goodness</i></span>. <span class="tex-span"><i>T</i>(<i>s</i>)</span> can be calculated as follows:</p><p>Consider there are exactly <span class="tex-span"><i>m</i></span> blocks of <span class="tex-span">1</span>s in this string (a block of <span class="tex-span">1</span>s in <span class="tex-span"><i>s</i></span> is a maximal consecutive substring of <span class="tex-span"><i>s</i></span> that only contains <span class="tex-span">1</span>) with lengths <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>m</i></sub></span>.</p><p>Define <img align="middle" class="tex-formula" src="file://ahn1kATj.png" style="max-width: 100.0%;max-height: 100.0%;"> where <span class="tex-span"><i>f</i></span> is a given sequence (if <span class="tex-span"><i>m</i> = 0</span>, then <span class="tex-span"><i>T</i>(<i>s</i>) = 0</span>).</p><p>Tavas loves queries. He asks you to answer <span class="tex-span"><i>q</i></span> queries. In each query he gives you numbers <span class="tex-span"><i>v</i>, <i>u</i>, <i>l</i></span> and you should print following number:</p><p>Consider the roads on the path from city <span class="tex-span"><i>v</i></span> to city <span class="tex-span"><i>u</i></span>: <span class="tex-span"><i>e</i><sub class="lower-index">1</sub>, <i>e</i><sub class="lower-index">2</sub>, ..., <i>e</i><sub class="lower-index"><i>x</i></sub></span>.</p><p>Build the binary string <span class="tex-span"><i>b</i></span> of length <span class="tex-span"><i>x</i></span> such that: <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> = 1</span> if and only if <span class="tex-span"><i>l</i> ≤ <i>w</i>(<i>e</i><sub class="lower-index"><i>i</i></sub>)</span> where <span class="tex-span"><i>w</i>(<i>e</i>)</span> is the length of road <span class="tex-span"><i>e</i></span>.</p><p>You should print <span class="tex-span"><i>T</i>(<i>b</i>)</span> for this query.</p></div><div class="input-specification"><p>The first line of input contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span> and <span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The next line contains <span class="tex-span"><i>n</i> - 1</span> space separated integers <span class="tex-span"><i>f</i><sub class="lower-index">1</sub>, <i>f</i><sub class="lower-index">2</sub>, ..., <i>f</i><sub class="lower-index"><i>n</i> - 1</sub></span> (<span class="tex-span">|<i>f</i><sub class="lower-index"><i>i</i></sub>| ≤ 1000</span>).</p><p>The next <span class="tex-span"><i>n</i> - 1</span> lines contain the details of the roads. Each line contains integers <span class="tex-span"><i>v</i>, <i>u</i></span> and <span class="tex-span"><i>w</i></span> and it means that there's a road between cities <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>u</i></span> of length <span class="tex-span"><i>w</i></span> (<span class="tex-span">1 ≤ <i>v</i>, <i>u</i> ≤ <i>n</i></span> and <span class="tex-span">1 ≤ <i>w</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The next <span class="tex-span"><i>q</i></span> lines contain the details of the queries. Each line contains integers <span class="tex-span"><i>v</i>, <i>u</i>, <i>l</i></span> (<span class="tex-span">1 ≤ <i>v</i>, <i>u</i> ≤ <i>n</i></span>, <span class="tex-span"><i>v</i> ≠ <i>u</i></span> and <span class="tex-span">1 ≤ <i>l</i> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print the answer of each query in a single line.</p></div>

## Input

<p>The first line of input contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span> and <span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The next line contains <span class="tex-span"><i>n</i> - 1</span> space separated integers <span class="tex-span"><i>f</i><sub class="lower-index">1</sub>, <i>f</i><sub class="lower-index">2</sub>, ..., <i>f</i><sub class="lower-index"><i>n</i> - 1</sub></span> (<span class="tex-span">|<i>f</i><sub class="lower-index"><i>i</i></sub>| ≤ 1000</span>).</p><p>The next <span class="tex-span"><i>n</i> - 1</span> lines contain the details of the roads. Each line contains integers <span class="tex-span"><i>v</i>, <i>u</i></span> and <span class="tex-span"><i>w</i></span> and it means that there's a road between cities <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>u</i></span> of length <span class="tex-span"><i>w</i></span> (<span class="tex-span">1 ≤ <i>v</i>, <i>u</i> ≤ <i>n</i></span> and <span class="tex-span">1 ≤ <i>w</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The next <span class="tex-span"><i>q</i></span> lines contain the details of the queries. Each line contains integers <span class="tex-span"><i>v</i>, <i>u</i>, <i>l</i></span> (<span class="tex-span">1 ≤ <i>v</i>, <i>u</i> ≤ <i>n</i></span>, <span class="tex-span"><i>v</i> ≠ <i>u</i></span> and <span class="tex-span">1 ≤ <i>l</i> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print the answer of each query in a single line.</p>





```input1
2 3
10
1 2 3
1 2 2
1 2 3
1 2 4

```




```input2
6 6
-5 0 0 2 10
1 2 1
2 3 2
3 4 5
4 5 1
5 6 5
1 6 1
1 6 2
1 6 5
3 6 5
4 6 4
1 4 2

```




```output1
10
10
0

```




```output2
10
-5
-10
-10
-5
0

```


