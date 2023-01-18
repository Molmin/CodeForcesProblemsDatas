## Description

<div><p>Ilya the Lion wants to help all his friends with passing exams. They need to solve the following problem to pass the IT exam.</p><p>You've got string <span class="tex-span"><i>s</i> = <i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"><i>n</i></span> is the length of the string), consisting only of characters "<span class="tex-font-style-tt">.</span>" and "<span class="tex-font-style-tt">#</span>" and <span class="tex-span"><i>m</i></span> queries. Each query is described by a pair of integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>. The answer to the query <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> is the number of such integers <span class="tex-span"><i>i</i></span> <span class="tex-span">(<i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>i</i> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub>)</span>, that <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> = <i>s</i><sub class="lower-index"><i>i</i> + 1</sub></span>.</p><p>Ilya the Lion wants to help his friends but is there anyone to help him? Help Ilya, solve the problem.</p></div><div class="input-specification"><p>The first line contains string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. It is guaranteed that the given string only consists of characters "<span class="tex-font-style-tt">.</span>" and "<span class="tex-font-style-tt">#</span>".</p><p>The next line contains integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of queries. Each of the next <span class="tex-span"><i>m</i></span> lines contains the description of the corresponding query. The <span class="tex-span"><i>i</i></span>-th line contains integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> integers — the answers to the queries in the order in which they are given in the input.</p></div>

## Input

<p>The first line contains string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. It is guaranteed that the given string only consists of characters "<span class="tex-font-style-tt">.</span>" and "<span class="tex-font-style-tt">#</span>".</p><p>The next line contains integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of queries. Each of the next <span class="tex-span"><i>m</i></span> lines contains the description of the corresponding query. The <span class="tex-span"><i>i</i></span>-th line contains integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> integers — the answers to the queries in the order in which they are given in the input.</p>





```input1
......
4
3 4
2 3
1 6
2 6

```




```input2
#..###
5
1 3
5 6
1 5
3 6
3 4

```




```output1
1
1
5
4

```




```output2
1
1
2
2
0

```


