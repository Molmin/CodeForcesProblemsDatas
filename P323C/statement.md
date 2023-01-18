## Description

<div><p>You are given two permutations <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span>, consisting of <span class="tex-span"><i>n</i></span> elements, and <span class="tex-span"><i>m</i></span> queries of the form: <span class="tex-span"><i>l</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">1</sub>, <i>l</i><sub class="lower-index">2</sub>, <i>r</i><sub class="lower-index">2</sub></span> <span class="tex-span">(<i>l</i><sub class="lower-index">1</sub> ≤ <i>r</i><sub class="lower-index">1</sub>;&nbsp;<i>l</i><sub class="lower-index">2</sub> ≤ <i>r</i><sub class="lower-index">2</sub>)</span>. The response for the query is the number of such integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, that their position in the first permutation is in segment <span class="tex-span">[<i>l</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">1</sub>]</span> (borders included), and position in the second permutation is in segment <span class="tex-span">[<i>l</i><sub class="lower-index">2</sub>, <i>r</i><sub class="lower-index">2</sub>]</span> (borders included too).</p><p>A <span class="tex-font-style-it">permutation</span> of <span class="tex-span"><i>n</i></span> elements is the sequence of <span class="tex-span"><i>n</i></span> distinct integers, each not less than <span class="tex-span">1</span> and not greater than <span class="tex-span"><i>n</i></span>.</p><p><span class="tex-font-style-it">Position</span> of number <span class="tex-span"><i>v</i></span> <span class="tex-span">(1 ≤ <i>v</i> ≤ <i>n</i>)</span> in permutation <span class="tex-span"><i>g</i><sub class="lower-index">1</sub>, <i>g</i><sub class="lower-index">2</sub>, ..., <i>g</i><sub class="lower-index"><i>n</i></sub></span> is such number <span class="tex-span"><i>i</i></span>, that <span class="tex-span"><i>g</i><sub class="lower-index"><i>i</i></sub> = <i>v</i></span>.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i> (1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>)</span>, the number of elements in both permutations. The following line contains <span class="tex-span"><i>n</i></span> integers, separated with spaces: <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub> (1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>. These are elements of the first permutation. The next line contains the second permutation <span class="tex-span"><i>q</i><sub class="lower-index">1</sub>, <i>q</i><sub class="lower-index">2</sub>, ..., <i>q</i><sub class="lower-index"><i>n</i></sub></span> in same format.</p><p>The following line contains an integer <span class="tex-span"><i>m</i> (1 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup>)</span>, that is the number of queries.</p><p>The following <span class="tex-span"><i>m</i></span> lines contain descriptions of queries one in a line. The description of the <span class="tex-span"><i>i</i></span>-th query consists of four integers: <span class="tex-span"><i>a</i>, <i>b</i>, <i>c</i>, <i>d</i> (1 ≤ <i>a</i>, <i>b</i>, <i>c</i>, <i>d</i> ≤ <i>n</i>)</span>. Query parameters <span class="tex-span"><i>l</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">1</sub>, <i>l</i><sub class="lower-index">2</sub>, <i>r</i><sub class="lower-index">2</sub></span> are obtained from the numbers <span class="tex-span"><i>a</i>, <i>b</i>, <i>c</i>, <i>d</i></span> using the following algorithm: </p><ol> <li> Introduce variable <span class="tex-span"><i>x</i></span>. If it is the first query, then the variable equals <span class="tex-span">0</span>, else it equals the response for the previous query plus one. </li><li> Introduce function <span class="tex-span"><i>f</i>(<i>z</i>) = ((<i>z</i> - 1 + <i>x</i>) <i>mod</i> <i>n</i>) + 1</span>. </li><li> Suppose <span class="tex-span"><i>l</i><sub class="lower-index">1</sub> = <i>min</i>(<i>f</i>(<i>a</i>), <i>f</i>(<i>b</i>)), <i>r</i><sub class="lower-index">1</sub> = <i>max</i>(<i>f</i>(<i>a</i>), <i>f</i>(<i>b</i>)), <i>l</i><sub class="lower-index">2</sub> = <i>min</i>(<i>f</i>(<i>c</i>), <i>f</i>(<i>d</i>)), <i>r</i><sub class="lower-index">2</sub> = <i>max</i>(<i>f</i>(<i>c</i>), <i>f</i>(<i>d</i>))</span>. </li></ol></div><div class="output-specification"><p>Print a response for each query in a separate line.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i> (1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>)</span>, the number of elements in both permutations. The following line contains <span class="tex-span"><i>n</i></span> integers, separated with spaces: <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub> (1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>. These are elements of the first permutation. The next line contains the second permutation <span class="tex-span"><i>q</i><sub class="lower-index">1</sub>, <i>q</i><sub class="lower-index">2</sub>, ..., <i>q</i><sub class="lower-index"><i>n</i></sub></span> in same format.</p><p>The following line contains an integer <span class="tex-span"><i>m</i> (1 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup>)</span>, that is the number of queries.</p><p>The following <span class="tex-span"><i>m</i></span> lines contain descriptions of queries one in a line. The description of the <span class="tex-span"><i>i</i></span>-th query consists of four integers: <span class="tex-span"><i>a</i>, <i>b</i>, <i>c</i>, <i>d</i> (1 ≤ <i>a</i>, <i>b</i>, <i>c</i>, <i>d</i> ≤ <i>n</i>)</span>. Query parameters <span class="tex-span"><i>l</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">1</sub>, <i>l</i><sub class="lower-index">2</sub>, <i>r</i><sub class="lower-index">2</sub></span> are obtained from the numbers <span class="tex-span"><i>a</i>, <i>b</i>, <i>c</i>, <i>d</i></span> using the following algorithm: </p><ol> <li> Introduce variable <span class="tex-span"><i>x</i></span>. If it is the first query, then the variable equals <span class="tex-span">0</span>, else it equals the response for the previous query plus one. </li><li> Introduce function <span class="tex-span"><i>f</i>(<i>z</i>) = ((<i>z</i> - 1 + <i>x</i>) <i>mod</i> <i>n</i>) + 1</span>. </li><li> Suppose <span class="tex-span"><i>l</i><sub class="lower-index">1</sub> = <i>min</i>(<i>f</i>(<i>a</i>), <i>f</i>(<i>b</i>)), <i>r</i><sub class="lower-index">1</sub> = <i>max</i>(<i>f</i>(<i>a</i>), <i>f</i>(<i>b</i>)), <i>l</i><sub class="lower-index">2</sub> = <i>min</i>(<i>f</i>(<i>c</i>), <i>f</i>(<i>d</i>)), <i>r</i><sub class="lower-index">2</sub> = <i>max</i>(<i>f</i>(<i>c</i>), <i>f</i>(<i>d</i>))</span>. </li></ol>

## Output

<p>Print a response for each query in a separate line.</p>





```input1
3
3 1 2
3 2 1
1
1 2 3 3

```




```input2
4
4 3 2 1
2 3 4 1
3
1 2 3 4
1 3 2 1
1 4 2 3

```




```output1
1

```




```output2
1
1
2

```


