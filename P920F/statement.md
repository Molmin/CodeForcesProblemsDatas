## Description

<div><p>Let <span class="tex-span"><i>D</i>(<i>x</i>)</span> be the number of positive divisors of a positive integer <span class="tex-span"><i>x</i></span>. For example, <span class="tex-span"><i>D</i>(2) = 2</span> (<span class="tex-span">2</span> is divisible by <span class="tex-span">1</span> and <span class="tex-span">2</span>), <span class="tex-span"><i>D</i>(6) = 4</span> (<span class="tex-span">6</span> is divisible by <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">3</span> and <span class="tex-span">6</span>).</p><p>You are given an array <span class="tex-span"><i>a</i></span> of <span class="tex-span"><i>n</i></span> integers. You have to process two types of queries:</p><ol> <li> <span class="tex-font-style-tt">REPLACE</span> <span class="tex-span"><i>l</i></span> <span class="tex-span"><i>r</i></span> — for every <img align="middle" class="tex-formula" src="file://3mkTqeZp.png" style="max-width: 100.0%;max-height: 100.0%;"> replace <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> with <span class="tex-span"><i>D</i>(<i>a</i><sub class="lower-index"><i>i</i></sub>)</span>; </li><li> <span class="tex-font-style-tt">SUM</span> <span class="tex-span"><i>l</i></span> <span class="tex-span"><i>r</i></span> — calculate <img align="middle" class="tex-formula" src="file://cCWswO0u.png" style="max-width: 100.0%;max-height: 100.0%;">. </li></ol><p>Print the answer for each <span class="tex-font-style-tt">SUM</span> query.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the number of elements in the array and the number of queries to process, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the elements of the array.</p><p>Then <span class="tex-span"><i>m</i></span> lines follow, each containing <span class="tex-span">3</span> integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> denoting <span class="tex-span"><i>i</i></span>-th query. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 1</span>, then <span class="tex-span"><i>i</i></span>-th query is <span class="tex-font-style-tt">REPLACE</span> <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, otherwise it's <span class="tex-font-style-tt">SUM</span> <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>, <span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p><p>There is at least one <span class="tex-font-style-tt">SUM</span> query.</p></div><div class="output-specification"><p>For each <span class="tex-font-style-tt">SUM</span> query print the answer to it.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the number of elements in the array and the number of queries to process, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the elements of the array.</p><p>Then <span class="tex-span"><i>m</i></span> lines follow, each containing <span class="tex-span">3</span> integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> denoting <span class="tex-span"><i>i</i></span>-th query. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 1</span>, then <span class="tex-span"><i>i</i></span>-th query is <span class="tex-font-style-tt">REPLACE</span> <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, otherwise it's <span class="tex-font-style-tt">SUM</span> <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>, <span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p><p>There is at least one <span class="tex-font-style-tt">SUM</span> query.</p>

## Output

<p>For each <span class="tex-font-style-tt">SUM</span> query print the answer to it.</p>





```input1
7 6
6 4 1 10 3 2 4
2 1 7
2 4 5
1 3 5
2 4 4
1 5 7
2 1 7

```




```output1
30
13
4
22

```


