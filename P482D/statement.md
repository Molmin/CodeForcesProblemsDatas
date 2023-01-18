## Description

<div><p>You have a rooted tree consisting of <span class="tex-span"><i>n</i></span> vertices. Let's number them with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> inclusive. The root of the tree is the vertex <span class="tex-span">1</span>. For each <span class="tex-span"><i>i</i> &gt; 1</span> direct parent of the vertex <span class="tex-span"><i>i</i></span> is <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>. We say that vertex <span class="tex-span"><i>i</i></span> is child for its direct parent <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>You have initially painted all the vertices with red color. You like to repaint some vertices of the tree. To perform painting you use the function <span class="tex-font-style-tt">paint</span> that you call with the root of the tree as an argument. Here is the pseudocode of this function:</p><pre class="verbatim"><br>count = 0 // global integer variable <br><br>rnd() { // this function is used in paint code<br>    return 0 or 1 equiprobably<br>}<br><br>paint(s) {<br>    if (count is even) then paint s with white color<br>    else paint s with black color<br><br>    count = count + 1<br>    <br>    if rnd() = 1 then children = [array of vertex s children in ascending order of their numbers]<br>    else children = [array of vertex s children in descending order of their numbers]<br><br>    for child in children { // iterating over children array<br>        if rnd() = 1 then paint(child) // calling paint recursively<br>    }<br>}<br></pre><p>As a result of this function, some vertices may change their colors to white or black and some of them may remain red.</p><p>Your task is to determine the number of distinct possible colorings of the vertices of the tree. We will assume that the coloring is possible if there is a nonzero probability to get this coloring with a single call of <span class="tex-span"><i>paint</i>(1)</span>. We assume that the colorings are different if there is a pair of vertices that are painted with different colors in these colorings. Since the required number may be very large, find its remainder of division by <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of vertexes in the tree.</p><p>The second line contains <span class="tex-span"><i>n</i> - 1</span> integers <span class="tex-span"><i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> &lt; <i>i</i></span>). Number <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is the parent of vertex <span class="tex-span"><i>i</i></span>.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the answer to the problem modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>)</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of vertexes in the tree.</p><p>The second line contains <span class="tex-span"><i>n</i> - 1</span> integers <span class="tex-span"><i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> &lt; <i>i</i></span>). Number <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is the parent of vertex <span class="tex-span"><i>i</i></span>.</p>

## Output

<p>Print a single integer&nbsp;— the answer to the problem modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>)</p>





```input1
4
1 2 1

```




```input2
3
1 1

```




```output1
8

```




```output2
5

```



## Note

<p>All possible coloring patterns of the first sample are given below.</p><center> <img class="tex-graphics" src="file://HM8sXSEj.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
