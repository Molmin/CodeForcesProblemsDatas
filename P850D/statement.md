## Description

<div><p>Ivan is reading a book about tournaments. He knows that a tournament is an oriented graph with exactly one oriented edge between each pair of vertices. The score of a vertex is the number of edges going outside this vertex. </p><p>Yesterday Ivan learned Landau's criterion: there is tournament with scores <span class="tex-span"><i>d</i><sub class="lower-index">1</sub> ≤ <i>d</i><sub class="lower-index">2</sub> ≤ ... ≤ <i>d</i><sub class="lower-index"><i>n</i></sub></span> if and only if <img align="middle" class="tex-formula" src="file://WBM3FQBi.png" style="max-width: 100.0%;max-height: 100.0%;"> for all <span class="tex-span">1 ≤ <i>k</i> &lt; <i>n</i></span> and <img align="middle" class="tex-formula" src="file://kK8c8Ga7.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Now, Ivan wanna solve following problem: given a <span class="tex-font-style-bf">set</span> of numbers <span class="tex-span"><i>S</i> = {<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub>}</span>, is there a tournament with given set of scores? I.e. is there tournament with sequence of scores <span class="tex-span"><i>d</i><sub class="lower-index">1</sub>, <i>d</i><sub class="lower-index">2</sub>, ..., <i>d</i><sub class="lower-index"><i>n</i></sub></span> such that if we remove duplicates in scores, we obtain the required set <span class="tex-span">{<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub>}</span>? </p><p>Find a tournament with <span class="tex-font-style-bf">minimum</span> possible number of vertices. </p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 31</span>).</p><p>The next line contains <span class="tex-span"><i>m</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 30</span>)&nbsp;— elements of the set <span class="tex-span"><i>S</i></span>. It is guaranteed that all elements of the set are distinct.</p></div><div class="output-specification"><p>If there are no such tournaments, print string "<span class="tex-font-style-tt">=(</span>" (without quotes).</p><p>Otherwise, print an integer <span class="tex-span"><i>n</i></span>&nbsp;— the number of vertices in the tournament.</p><p>Then print <span class="tex-span"><i>n</i></span> lines with <span class="tex-span"><i>n</i></span> characters&nbsp;— matrix of the tournament. The <span class="tex-span"><i>j</i></span>-th element in the <span class="tex-span"><i>i</i></span>-th row should be <span class="tex-span">1</span> if the edge between the <span class="tex-span"><i>i</i></span>-th and the <span class="tex-span"><i>j</i></span>-th vertices is oriented towards the <span class="tex-span"><i>j</i></span>-th vertex, and <span class="tex-span">0</span> otherwise. The main diagonal should contain only zeros.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 31</span>).</p><p>The next line contains <span class="tex-span"><i>m</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 30</span>)&nbsp;— elements of the set <span class="tex-span"><i>S</i></span>. It is guaranteed that all elements of the set are distinct.</p>

## Output

<p>If there are no such tournaments, print string "<span class="tex-font-style-tt">=(</span>" (without quotes).</p><p>Otherwise, print an integer <span class="tex-span"><i>n</i></span>&nbsp;— the number of vertices in the tournament.</p><p>Then print <span class="tex-span"><i>n</i></span> lines with <span class="tex-span"><i>n</i></span> characters&nbsp;— matrix of the tournament. The <span class="tex-span"><i>j</i></span>-th element in the <span class="tex-span"><i>i</i></span>-th row should be <span class="tex-span">1</span> if the edge between the <span class="tex-span"><i>i</i></span>-th and the <span class="tex-span"><i>j</i></span>-th vertices is oriented towards the <span class="tex-span"><i>j</i></span>-th vertex, and <span class="tex-span">0</span> otherwise. The main diagonal should contain only zeros.</p>





```input1
2
1 2

```




```input2
2
0 3

```




```output1
4
0011
1001
0100
0010

```




```output2
6
000111
100011
110001
011001
001101
000000

```


