## Description

<div><p>PolandBall lives in a forest with his family. There are some trees in the forest. Trees are undirected acyclic graphs with <span class="tex-span"><i>k</i></span> vertices and <span class="tex-span"><i>k</i> - 1</span> edges, where <span class="tex-span"><i>k</i></span> is some integer. Note that one vertex <span class="tex-font-style-bf">is</span> a valid tree.</p><p>There is exactly one relative living in each vertex of each tree, they have unique ids from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. For each Ball <span class="tex-span"><i>i</i></span> we know the id of its most distant relative living on the same tree. If there are several such vertices, we only know the value of the one with smallest id among those.</p><p>How many trees are there in the forest?</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup></span>)&nbsp;— the number of Balls living in the forest.</p><p>The second line contains a sequence <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> of length <span class="tex-span"><i>n</i></span>, where (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) holds and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> denotes the most distant from Ball <span class="tex-span"><i>i</i></span> relative living on the same tree. If there are several most distant relatives living on the same tree, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is the id of one with the smallest id.</p><p>It's guaranteed that the sequence <span class="tex-span"><i>p</i></span> corresponds to some valid forest.</p><p><span class="tex-font-style-bf">Hacking</span>: To hack someone, you should provide a <span class="tex-font-style-bf">correct forest</span> as a test. The sequence <span class="tex-span"><i>p</i></span> will be calculated according to the forest and given to the solution you try to hack as input. Use the following format:</p><p>In the first line, output the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup></span>)&nbsp;— the number of Balls and the integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>m</i> &lt; <i>n</i></span>)&nbsp;— the total number of edges in the forest. Then <span class="tex-span"><i>m</i></span> lines should follow. The <span class="tex-span"><i>i</i></span>-th of them should contain two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and represent an edge between vertices in which relatives <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> live. For example, the first sample is written as follows:</p><pre class="verbatim"><br>5 3<br>1 2<br>3 4<br>4 5<br></pre></div><div class="output-specification"><p>You should output the number of trees in the forest where PolandBall lives.</p></div><div><h2>Interaction</h2><p>From the technical side, this problem is interactive. However, it should not affect you (except hacking) since there is no interaction.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup></span>)&nbsp;— the number of Balls living in the forest.</p><p>The second line contains a sequence <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> of length <span class="tex-span"><i>n</i></span>, where (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) holds and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> denotes the most distant from Ball <span class="tex-span"><i>i</i></span> relative living on the same tree. If there are several most distant relatives living on the same tree, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is the id of one with the smallest id.</p><p>It's guaranteed that the sequence <span class="tex-span"><i>p</i></span> corresponds to some valid forest.</p><p><span class="tex-font-style-bf">Hacking</span>: To hack someone, you should provide a <span class="tex-font-style-bf">correct forest</span> as a test. The sequence <span class="tex-span"><i>p</i></span> will be calculated according to the forest and given to the solution you try to hack as input. Use the following format:</p><p>In the first line, output the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup></span>)&nbsp;— the number of Balls and the integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>m</i> &lt; <i>n</i></span>)&nbsp;— the total number of edges in the forest. Then <span class="tex-span"><i>m</i></span> lines should follow. The <span class="tex-span"><i>i</i></span>-th of them should contain two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and represent an edge between vertices in which relatives <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> live. For example, the first sample is written as follows:</p><pre class="verbatim"><br>5 3<br>1 2<br>3 4<br>4 5<br></pre>

## Output

<p>You should output the number of trees in the forest where PolandBall lives.</p>





```input1
5
2 1 5 3 3
```




```input2
1
1

```




```output1
2
```




```output2
1
```



## Note

<p>In the first sample testcase, possible forest is: <span class="tex-font-style-tt">1-2 3-4-5</span>. </p><p>There are <span class="tex-span">2</span> trees overall.</p><p>In the second sample testcase, the only possible graph is one vertex and no edges. Therefore, there is only one tree.</p>
