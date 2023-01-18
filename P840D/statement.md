## Description

<div><p>Once, Leha found in the left pocket an array consisting of <span class="tex-span"><i>n</i></span> integers, and in the right pocket <span class="tex-span"><i>q</i></span> queries of the form <span class="tex-span"><i>l</i></span> <span class="tex-span"><i>r</i></span> <span class="tex-span"><i>k</i></span>. If there are queries, then they must be answered. Answer for the query is minimal <span class="tex-span"><i>x</i></span> such that <span class="tex-span"><i>x</i></span> occurs in the interval <span class="tex-span"><i>l</i></span> <span class="tex-span"><i>r</i></span> strictly more than <img align="middle" class="tex-formula" src="file://dnVw0Hpy.png" style="max-width: 100.0%;max-height: 100.0%;"> times or <span class="tex-span"> - 1</span> if there is no such number. Help Leha with such a difficult task.</p></div><div class="input-specification"><p>First line of input data contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>q</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — number of elements in the array and number of queries respectively.</p><p>Next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — Leha's array.</p><p>Each of next <span class="tex-span"><i>q</i></span> lines contains three integers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i>, 2 ≤ <i>k</i> ≤ 5</span>) — description of the queries.</p></div><div class="output-specification"><p>Output answer for each query in new line.</p></div>

## Input

<p>First line of input data contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>q</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — number of elements in the array and number of queries respectively.</p><p>Next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — Leha's array.</p><p>Each of next <span class="tex-span"><i>q</i></span> lines contains three integers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i>, 2 ≤ <i>k</i> ≤ 5</span>) — description of the queries.</p>

## Output

<p>Output answer for each query in new line.</p>





```input1
4 2
1 1 2 2
1 3 2
1 4 2

```




```input2
5 3
1 2 1 3 2
2 5 3
1 2 3
5 5 2

```




```output1
1
-1

```




```output2
2
1
2

```


