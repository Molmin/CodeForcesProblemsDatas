## Description

<div><p>Limak is a little bear who learns to draw. People usually start with houses, fences and flowers but why would bears do it? Limak lives in the forest and he decides to draw a tree.</p><p>Recall that <span class="tex-font-style-it">tree</span> is a connected graph consisting of <span class="tex-span"><i>n</i></span> vertices and <span class="tex-span"><i>n</i> - 1</span> edges.</p><p>Limak chose a tree with <span class="tex-span"><i>n</i></span> vertices. He has infinite strip of paper with two parallel rows of dots. Little bear wants to assign vertices of a tree to some <span class="tex-span"><i>n</i></span> distinct dots on a paper so that edges would intersect only at their endpoints — drawn tree must be planar. Below you can see one of correct drawings for the first sample test.</p><center> <img class="tex-graphics" src="file://lGq3pb5c.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Is it possible for Limak to draw chosen tree?</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>Next <span class="tex-span"><i>n</i> - 1</span> lines contain description of a tree. <span class="tex-span"><i>i</i></span>-th of them contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>) denoting an edge between vertices <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. It's guaranteed that given description forms a tree.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">Yes</span>" (without the quotes) if Limak can draw chosen tree. Otherwise, print "<span class="tex-font-style-tt">No</span>" (without the quotes).</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>Next <span class="tex-span"><i>n</i> - 1</span> lines contain description of a tree. <span class="tex-span"><i>i</i></span>-th of them contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>) denoting an edge between vertices <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. It's guaranteed that given description forms a tree.</p>

## Output

<p>Print "<span class="tex-font-style-tt">Yes</span>" (without the quotes) if Limak can draw chosen tree. Otherwise, print "<span class="tex-font-style-tt">No</span>" (without the quotes).</p>





```input1
8
1 2
1 3
1 6
6 4
6 7
6 5
7 8

```




```input2
13
1 2
1 3
1 4
2 5
2 6
2 7
3 8
3 9
3 10
4 11
4 12
4 13

```




```output1
Yes

```




```output2
No

```


