## Description

<div><p>You have an array <span class="tex-span"><i>f</i></span> of <span class="tex-span"><i>n</i></span> functions.The function <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub>(<i>x</i>)</span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) is characterized by parameters: <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>a</i>, <i>b</i>, <i>y</i><sub class="lower-index">2</sub></span> and take values: </p><ul> <li> <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, if <span class="tex-span"><i>x</i> ≤ <i>x</i><sub class="lower-index">1</sub></span>. </li><li> <span class="tex-span"><i>a</i>·<i>x</i> + <i>b</i></span>, if <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> &lt; <i>x</i> ≤ <i>x</i><sub class="lower-index">2</sub></span>. </li><li> <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span>, if <span class="tex-span"><i>x</i> &gt; <i>x</i><sub class="lower-index">2</sub></span>. </li></ul><p>There are <span class="tex-span"><i>m</i></span> queries. Each query is determined by numbers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>x</i></span>. For a query with number <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>m</i></span>), you need to calculate the sum of all <span class="tex-span"><i>f</i><sub class="lower-index"><i>j</i></sub>(<i>x</i><sub class="lower-index"><i>i</i></sub>)</span> where <span class="tex-span"><i>l</i> ≤ <i>j</i> ≤ <i>r</i></span>. The value of <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> is calculated as follows: <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> = (<i>x</i> + <i>last</i>)</span> mod <span class="tex-span">10<sup class="upper-index">9</sup></span>, where <span class="tex-span"><i>last</i></span> is the answer to the query with number <span class="tex-span"><i>i</i> - 1</span>. The value of <span class="tex-span"><i>last</i></span> equals <span class="tex-span">0</span> if <span class="tex-span"><i>i</i> = 1</span>.</p></div><div class="input-specification"><p>First line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 75000</span>).</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains six integer numbers: <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>a</i>, <i>b</i>, <i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index">1</sub> &lt; <i>x</i><sub class="lower-index">2</sub> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">4</sup></span>).</p><p>Next line contains one integer number <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 500000</span>).</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains three integer numbers: <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>).</p></div>

## Input

<p>First line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 75000</span>).</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains six integer numbers: <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>a</i>, <i>b</i>, <i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index">1</sub> &lt; <i>x</i><sub class="lower-index">2</sub> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">4</sup></span>).</p><p>Next line contains one integer number <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 500000</span>).</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains three integer numbers: <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>).</p>





```input1
1
1 2 1 4 5 10
1
1 1 2

```




```input2
3
2 5 1 1 1 4
3 6 8 2 5 7
1 3 5 1 4 10
3
1 3 3
2 3 2
1 2 5

```




```output1
13

```




```output2
19
17
11

```


