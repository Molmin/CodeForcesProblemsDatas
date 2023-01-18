## Description

<div><p><span class="tex-font-style-underline">Karafs is some kind of vegetable in shape of an <span class="tex-span">1 × <i>h</i></span> rectangle. Tavaspolis people love Karafs and they use Karafs in almost any kind of food. Tavas, himself, is crazy about Karafs.</span></p><center> <img class="tex-graphics" src="file://4Yc50bP0.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Each Karafs has a positive integer height. Tavas has an infinite <span class="tex-font-style-bf">1-based</span> sequence of Karafses. The height of the <span class="tex-span"><i>i</i></span>-th Karafs is <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> = <i>A</i> + (<i>i</i> - 1) × <i>B</i></span>.</p><p>For a given <span class="tex-span"><i>m</i></span>, let's define an <span class="tex-span"><i>m</i></span>-bite operation as decreasing the height of at most <span class="tex-span"><i>m</i></span> distinct not eaten Karafses by 1. Karafs is considered as eaten when its height becomes zero.</p><p>Now SaDDas asks you <span class="tex-span"><i>n</i></span> queries. In each query he gives you numbers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>t</i></span> and <span class="tex-span"><i>m</i></span> and you should find the largest number <span class="tex-span"><i>r</i></span> such that <span class="tex-span"><i>l</i> ≤ <i>r</i></span> and sequence <span class="tex-span"><i>s</i><sub class="lower-index"><i>l</i></sub>, <i>s</i><sub class="lower-index"><i>l</i> + 1</sub>, ..., <i>s</i><sub class="lower-index"><i>r</i></sub></span> can be eaten <span class="tex-font-style-bf">by performing <span class="tex-span"><i>m</i></span>-bite no more than <span class="tex-span"><i>t</i></span> times</span> or print -1 if there is no such number <span class="tex-span"><i>r</i></span>.</p></div><div class="input-specification"><p>The first line of input contains three integers <span class="tex-span"><i>A</i></span>, <span class="tex-span"><i>B</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>A</i>, <i>B</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>Next <span class="tex-span"><i>n</i></span> lines contain information about queries. <span class="tex-span"><i>i</i></span>-th line contains integers <span class="tex-span"><i>l</i>, <i>t</i>, <i>m</i></span> (<span class="tex-span">1 ≤ <i>l</i>, <i>t</i>, <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>) for <span class="tex-span"><i>i</i></span>-th query.</p></div><div class="output-specification"><p>For each query, print its answer in a single line.</p></div>

## Input

<p>The first line of input contains three integers <span class="tex-span"><i>A</i></span>, <span class="tex-span"><i>B</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>A</i>, <i>B</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>Next <span class="tex-span"><i>n</i></span> lines contain information about queries. <span class="tex-span"><i>i</i></span>-th line contains integers <span class="tex-span"><i>l</i>, <i>t</i>, <i>m</i></span> (<span class="tex-span">1 ≤ <i>l</i>, <i>t</i>, <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>) for <span class="tex-span"><i>i</i></span>-th query.</p>

## Output

<p>For each query, print its answer in a single line.</p>





```input1
2 1 4
1 5 3
3 3 10
7 10 2
6 4 8

```




```input2
1 5 2
1 5 10
2 7 4

```




```output1
4
-1
8
-1

```




```output2
1
2

```


