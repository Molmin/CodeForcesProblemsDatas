## Description

<div><p>Aryo has got a lot of intervals for his <span class="tex-span">2418</span>th birthday. He is really excited and decided to color all these intervals with some colors. He has a simple rule for himself. He calls a coloring nice if there exists <span class="tex-font-style-underline">no</span> three intervals <span class="tex-span"><i>a</i>, <i>b</i></span> and <span class="tex-span"><i>c</i></span> such that the following conditions are satisfied simultaneously: </p><ul> <li> <span class="tex-span"><i>a</i>, <i>b</i></span> and <span class="tex-span"><i>c</i></span> are colored with the same color, </li><li> <img align="middle" class="tex-formula" src="file://66zQfTbp.png" style="max-width: 100.0%;max-height: 100.0%;">, </li><li> <img align="middle" class="tex-formula" src="file://mVGWr4eM.png" style="max-width: 100.0%;max-height: 100.0%;">, </li><li> <img align="middle" class="tex-formula" src="file://8476XIcn.png" style="max-width: 100.0%;max-height: 100.0%;">. </li></ul><p>Moreover he found out that for every intervals <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span>, there is at least one point in <span class="tex-span"><i>i</i></span> which isn't in <span class="tex-span"><i>j</i></span>.</p><p>Given some set of intervals. You have to find the minimum number <span class="tex-span"><i>k</i></span>, such that Aryo can find a nice coloring with <span class="tex-span"><i>k</i></span> colors.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup></span>), number of intervals.</p><p>The following <span class="tex-span"><i>n</i></span> lines contain a interval description each. Each interval is described by two numbers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub>, <i>e</i><sub class="lower-index"><i>i</i></sub></span> which are the start and end points of it (<span class="tex-span"> - 10<sup class="upper-index">5</sup> &lt; <i>s</i><sub class="lower-index"><i>i</i></sub>, <i>e</i><sub class="lower-index"><i>i</i></sub> &lt; 10<sup class="upper-index">5</sup></span>, <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> ≤ <i>e</i><sub class="lower-index"><i>i</i></sub></span>). See samples for clarity. A square bracket stands for including of the corresponding endpoint, while a round bracket stands for excluding.</p></div><div class="output-specification"><p>Write a single integer <span class="tex-span"><i>k</i></span> — the minimum number of colors needed for a nice coloring.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup></span>), number of intervals.</p><p>The following <span class="tex-span"><i>n</i></span> lines contain a interval description each. Each interval is described by two numbers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub>, <i>e</i><sub class="lower-index"><i>i</i></sub></span> which are the start and end points of it (<span class="tex-span"> - 10<sup class="upper-index">5</sup> &lt; <i>s</i><sub class="lower-index"><i>i</i></sub>, <i>e</i><sub class="lower-index"><i>i</i></sub> &lt; 10<sup class="upper-index">5</sup></span>, <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> ≤ <i>e</i><sub class="lower-index"><i>i</i></sub></span>). See samples for clarity. A square bracket stands for including of the corresponding endpoint, while a round bracket stands for excluding.</p>

## Output

<p>Write a single integer <span class="tex-span"><i>k</i></span> — the minimum number of colors needed for a nice coloring.</p>





```input1
2
[1,2)
(3,4]

```




```input2
3
[1,3]
[2,6]
(5,7)

```




```output1
1

```




```output2
2

```


