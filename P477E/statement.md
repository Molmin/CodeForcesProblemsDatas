## Description

<div><p>Dreamoon has just created a document of hard problems using notepad.exe. The document consists of <span class="tex-span"><i>n</i></span> lines of text, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> denotes the length of the <span class="tex-span"><i>i</i></span>-th line. He now wants to know what is the fastest way to move the cursor around because the document is really long.</p><p>Let <span class="tex-span">(<i>r</i>, <i>c</i>)</span> be a current cursor position, where <span class="tex-span"><i>r</i></span> is row number and <span class="tex-span"><i>c</i></span> is position of cursor in the row. We have <span class="tex-span">1 ≤ <i>r</i> ≤ <i>n</i></span> and <span class="tex-span">0 ≤ <i>c</i> ≤ <i>a</i><sub class="lower-index"><i>r</i></sub></span>.</p><p>We can use following six operations in notepad.exe to move our cursor assuming the current cursor position is at <span class="tex-span">(<i>r</i>, <i>c</i>)</span>:</p><ol> <li> up key: the new cursor position <span class="tex-span">(<i>nr</i>, <i>nc</i>) = (<i>max</i>(<i>r</i> - 1, 1), <i>min</i>(<i>a</i><sub class="lower-index"><i>nr</i></sub>, <i>c</i>))</span> </li><li> down key: the new cursor position <span class="tex-span">(<i>nr</i>, <i>nc</i>) = (<i>min</i>(<i>r</i> + 1, <i>n</i>), <i>min</i>(<i>a</i><sub class="lower-index"><i>nr</i></sub>, <i>c</i>))</span> </li><li> left key: the new cursor position <span class="tex-span">(<i>nr</i>, <i>nc</i>) = (<i>r</i>, <i>max</i>(0, <i>c</i> - 1))</span> </li><li> right key: the new cursor position <span class="tex-span">(<i>nr</i>, <i>nc</i>) = (<i>r</i>, <i>min</i>(<i>a</i><sub class="lower-index"><i>nr</i></sub>, <i>c</i> + 1))</span> </li><li> HOME key: the new cursor position <span class="tex-span">(<i>nr</i>, <i>nc</i>) = (<i>r</i>, 0)</span> </li><li> END key: the new cursor position <span class="tex-span">(<i>nr</i>, <i>nc</i>) = (<i>r</i>, <i>a</i><sub class="lower-index"><i>r</i></sub>)</span> </li></ol><p>You're given the document description (<span class="tex-span"><i>n</i></span> and sequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>) and <span class="tex-span"><i>q</i></span> queries from Dreamoon. Each query asks what minimal number of key presses is needed to move the cursor from <span class="tex-span">(<i>r</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">1</sub>)</span> to <span class="tex-span">(<i>r</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">2</sub>)</span>.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i>(1 ≤ <i>n</i> ≤ 400, 000)</span> — the number of lines of text. </p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup>)</span>.</p><p>The third line contains an integer <span class="tex-span"><i>q</i>(1 ≤ <i>q</i> ≤ 400, 000)</span>. </p><p>Each of the next <span class="tex-span"><i>q</i></span> lines contains four integers <span class="tex-span"><i>r</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">2</sub></span> representing a query (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub> ≤ <i>n</i>, 0 ≤ <i>c</i><sub class="lower-index">1</sub> ≤ <i>a</i><sub class="lower-index"><i>r</i>1</sub>, 0 ≤ <i>c</i><sub class="lower-index">2</sub> ≤ <i>a</i><sub class="lower-index"><i>r</i>2</sub></span>).</p></div><div class="output-specification"><p>For each query print the result of the query.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i>(1 ≤ <i>n</i> ≤ 400, 000)</span> — the number of lines of text. </p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup>)</span>.</p><p>The third line contains an integer <span class="tex-span"><i>q</i>(1 ≤ <i>q</i> ≤ 400, 000)</span>. </p><p>Each of the next <span class="tex-span"><i>q</i></span> lines contains four integers <span class="tex-span"><i>r</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">2</sub></span> representing a query (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub> ≤ <i>n</i>, 0 ≤ <i>c</i><sub class="lower-index">1</sub> ≤ <i>a</i><sub class="lower-index"><i>r</i>1</sub>, 0 ≤ <i>c</i><sub class="lower-index">2</sub> ≤ <i>a</i><sub class="lower-index"><i>r</i>2</sub></span>).</p>

## Output

<p>For each query print the result of the query.</p>





```input1
9
1 3 5 3 1 3 5 3 1
4
3 5 3 1
3 3 7 3
1 0 3 3
6 0 7 3

```




```input2
2
10 5
1
1 0 1 5

```




```output1
2
5
3
2

```




```output2
3

```



## Note

<p>In the first sample, the first query can be solved with keys: HOME, right.</p><p>The second query can be solved with keys: down, down, down, END, down.</p><p>The third query can be solved with keys: down, END, down.</p><p>The fourth query can be solved with keys: END, down.</p>
