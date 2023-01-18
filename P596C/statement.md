## Description

<div><p>Wilbur is playing with a set of <span class="tex-span"><i>n</i></span> points on the coordinate plane. All points have non-negative integer coordinates. Moreover, if some point (<span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>) belongs to the set, then all points (<span class="tex-span"><i>x</i>'</span>, <span class="tex-span"><i>y</i>'</span>), such that <span class="tex-span">0 ≤ <i>x</i>' ≤ <i>x</i></span> and <span class="tex-span">0 ≤ <i>y</i>' ≤ <i>y</i></span> also belong to this set.</p><p>Now Wilbur wants to number the points in the set he has, that is assign them distinct integer numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. In order to make the numbering <span class="tex-font-style-it">aesthetically pleasing</span>, Wilbur imposes the condition that if some point (<span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>) gets number <span class="tex-span"><i>i</i></span>, then all (<span class="tex-span"><i>x</i>'</span>,<span class="tex-span"><i>y</i>'</span>) from the set, such that <span class="tex-span"><i>x</i>' ≥ <i>x</i></span> and <span class="tex-span"><i>y</i>' ≥ <i>y</i></span> must be assigned a number not less than <span class="tex-span"><i>i</i></span>. For example, for a set of four points (<span class="tex-span">0</span>, <span class="tex-span">0</span>), (<span class="tex-span">0</span>, <span class="tex-span">1</span>), (<span class="tex-span">1</span>, <span class="tex-span">0</span>) and (<span class="tex-span">1</span>, <span class="tex-span">1</span>), there are two aesthetically pleasing numberings. One is <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">3</span>, <span class="tex-span">4</span> and another one is <span class="tex-span">1</span>, <span class="tex-span">3</span>, <span class="tex-span">2</span>, <span class="tex-span">4</span>.</p><p>Wilbur's friend comes along and challenges Wilbur. For any point he defines it's <span class="tex-font-style-it">special value</span> as <span class="tex-span"><i>s</i>(<i>x</i>, <i>y</i>) = <i>y</i> - <i>x</i></span>. Now he gives Wilbur some <span class="tex-span"><i>w</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>w</i><sub class="lower-index">2</sub></span>,..., <span class="tex-span"><i>w</i><sub class="lower-index"><i>n</i></sub></span>, and asks him to find an aesthetically pleasing numbering of the points in the set, such that the point that gets number <span class="tex-span"><i>i</i></span> has it's special value equal to <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>, that is <span class="tex-span"><i>s</i>(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>) = <i>y</i><sub class="lower-index"><i>i</i></sub> - <i>x</i><sub class="lower-index"><i>i</i></sub> = <i>w</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Now Wilbur asks you to help him with this challenge.</p></div><div class="input-specification"><p>The first line of the input consists of a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of points in the set Wilbur is playing with.</p><p>Next follow <span class="tex-span"><i>n</i></span> lines with points descriptions. Each line contains two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">0 ≤ <i>x</i>, <i>y</i> ≤ 100 000</span>), that give one point in Wilbur's set. It's guaranteed that all points are distinct. Also, it is guaranteed that if some point (<span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>) is present in the input, then all points (<span class="tex-span"><i>x</i>'</span>, <span class="tex-span"><i>y</i>'</span>), such that <span class="tex-span">0 ≤ <i>x</i>' ≤ <i>x</i></span> and <span class="tex-span">0 ≤ <i>y</i>' ≤ <i>y</i></span>, are also present in the input.</p><p>The last line of the input contains <span class="tex-span"><i>n</i></span> integers. The <span class="tex-span"><i>i</i></span>-th of them is <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 100 000 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>)&nbsp;— the required special value of the point that gets number <span class="tex-span"><i>i</i></span> in any aesthetically pleasing numbering.</p></div><div class="output-specification"><p>If there exists an aesthetically pleasant numbering of points in the set, such that <span class="tex-span"><i>s</i>(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>) = <i>y</i><sub class="lower-index"><i>i</i></sub> - <i>x</i><sub class="lower-index"><i>i</i></sub> = <i>w</i><sub class="lower-index"><i>i</i></sub></span>, then print "<span class="tex-font-style-tt">YES</span>" on the first line of the output. Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p><p>If a solution exists, proceed output with <span class="tex-span"><i>n</i></span> lines. On the <span class="tex-span"><i>i</i></span>-th of these lines print the point of the set that gets number <span class="tex-span"><i>i</i></span>. If there are multiple solutions, print any of them.</p></div>

## Input

<p>The first line of the input consists of a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of points in the set Wilbur is playing with.</p><p>Next follow <span class="tex-span"><i>n</i></span> lines with points descriptions. Each line contains two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">0 ≤ <i>x</i>, <i>y</i> ≤ 100 000</span>), that give one point in Wilbur's set. It's guaranteed that all points are distinct. Also, it is guaranteed that if some point (<span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>) is present in the input, then all points (<span class="tex-span"><i>x</i>'</span>, <span class="tex-span"><i>y</i>'</span>), such that <span class="tex-span">0 ≤ <i>x</i>' ≤ <i>x</i></span> and <span class="tex-span">0 ≤ <i>y</i>' ≤ <i>y</i></span>, are also present in the input.</p><p>The last line of the input contains <span class="tex-span"><i>n</i></span> integers. The <span class="tex-span"><i>i</i></span>-th of them is <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 100 000 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>)&nbsp;— the required special value of the point that gets number <span class="tex-span"><i>i</i></span> in any aesthetically pleasing numbering.</p>

## Output

<p>If there exists an aesthetically pleasant numbering of points in the set, such that <span class="tex-span"><i>s</i>(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>) = <i>y</i><sub class="lower-index"><i>i</i></sub> - <i>x</i><sub class="lower-index"><i>i</i></sub> = <i>w</i><sub class="lower-index"><i>i</i></sub></span>, then print "<span class="tex-font-style-tt">YES</span>" on the first line of the output. Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p><p>If a solution exists, proceed output with <span class="tex-span"><i>n</i></span> lines. On the <span class="tex-span"><i>i</i></span>-th of these lines print the point of the set that gets number <span class="tex-span"><i>i</i></span>. If there are multiple solutions, print any of them.</p>





```input1
5
2 0
0 0
1 0
1 1
0 1
0 -1 -2 1 0

```




```input2
3
1 0
0 0
2 0
0 1 2

```




```output1
YES
0 0
1 0
2 0
0 1
1 1

```




```output2
NO

```



## Note

<p>In the first sample, point (<span class="tex-span">2</span>, <span class="tex-span">0</span>) gets number <span class="tex-span">3</span>, point (<span class="tex-span">0</span>, <span class="tex-span">0</span>) gets number one, point (<span class="tex-span">1</span>, <span class="tex-span">0</span>) gets number <span class="tex-span">2</span>, point (<span class="tex-span">1</span>, <span class="tex-span">1</span>) gets number <span class="tex-span">5</span> and point (<span class="tex-span">0</span>, <span class="tex-span">1</span>) gets number <span class="tex-span">4</span>. One can easily check that this numbering is aesthetically pleasing and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub> - <i>x</i><sub class="lower-index"><i>i</i></sub> = <i>w</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>In the second sample, the special values of the points in the set are <span class="tex-span">0</span>, <span class="tex-span"> - 1</span>, and <span class="tex-span"> - 2</span> while the sequence that the friend gives to Wilbur is <span class="tex-span">0</span>, <span class="tex-span">1</span>, <span class="tex-span">2</span>. Therefore, the answer does not exist.</p>
