## Description

<div><p>You are given a tree (a connected non-oriented graph without cycles) with vertices numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, and the length of the <span class="tex-span"><i>i</i></span>-th edge is <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>. In the vertex <span class="tex-span"><i>s</i></span> there is a policeman, in the vertices <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub> ≠ <i>s</i></span>) <span class="tex-span"><i>m</i></span> criminals are located.</p><p>The policeman can walk along the edges with speed <span class="tex-span">1</span>, the criminals can move with arbitrary large speed. If a criminal at some moment is at the same point as the policeman, he instantly gets caught by the policeman. Determine the time needed for the policeman to catch all criminals, assuming everybody behaves optimally (i.e. the criminals maximize that time, the policeman minimizes that time). Everybody knows positions of everybody else at any moment of time.</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>)&nbsp;— the number of vertices in the tree. The next <span class="tex-span"><i>n</i> - 1</span> lines contain three integers each: <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 50</span>) denoting edges and their lengths. It is guaranteed that the given graph is a tree.</p><p>The next line contains single integer <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ <i>s</i> ≤ <i>n</i></span>)&nbsp;— the number of vertex where the policeman starts.</p><p>The next line contains single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 50</span>)&nbsp;— the number of criminals. The next line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub> ≠ <i>s</i></span>)&nbsp;— the number of vertices where the criminals are located. <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span> are not necessarily distinct.</p></div><div class="output-specification"><p>If the policeman can't catch criminals, print single line "<span class="tex-font-style-tt">Terrorists win</span>" (without quotes).</p><p>Otherwise, print single integer&nbsp;— the time needed to catch all criminals.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>)&nbsp;— the number of vertices in the tree. The next <span class="tex-span"><i>n</i> - 1</span> lines contain three integers each: <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 50</span>) denoting edges and their lengths. It is guaranteed that the given graph is a tree.</p><p>The next line contains single integer <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ <i>s</i> ≤ <i>n</i></span>)&nbsp;— the number of vertex where the policeman starts.</p><p>The next line contains single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 50</span>)&nbsp;— the number of criminals. The next line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub> ≠ <i>s</i></span>)&nbsp;— the number of vertices where the criminals are located. <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span> are not necessarily distinct.</p>

## Output

<p>If the policeman can't catch criminals, print single line "<span class="tex-font-style-tt">Terrorists win</span>" (without quotes).</p><p>Otherwise, print single integer&nbsp;— the time needed to catch all criminals.</p>





```input1
4
1 2 2
1 3 1
1 4 1
2
4
3 1 4 1

```




```input2
6
1 2 3
2 3 5
3 4 1
3 5 4
2 6 3
2
3
1 3 5

```




```output1
8

```




```output2
21

```



## Note

<p>In the first example one of the optimal scenarios is the following. The criminal number <span class="tex-span">2</span> moves to vertex <span class="tex-span">3</span>, the criminal <span class="tex-span">4</span>&nbsp;— to vertex <span class="tex-span">4</span>. The policeman goes to vertex <span class="tex-span">4</span> and catches two criminals. After that the criminal number <span class="tex-span">1</span> moves to the vertex <span class="tex-span">2</span>. The policeman goes to vertex <span class="tex-span">3</span> and catches criminal <span class="tex-span">2</span>, then goes to the vertex <span class="tex-span">2</span> and catches the remaining criminal.</p>
