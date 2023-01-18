## Description

<div><p>Dr. Evil is interested in math and functions, so he gave Mahmoud and Ehab array <span class="tex-span"><i>a</i></span> of length <span class="tex-span"><i>n</i></span> and array <span class="tex-span"><i>b</i></span> of length <span class="tex-span"><i>m</i></span>. He introduced a function <span class="tex-span"><i>f</i>(<i>j</i>)</span> which is defined for integers <span class="tex-span"><i>j</i></span>, which satisfy <span class="tex-span">0 ≤ <i>j</i> ≤ <i>m</i> - <i>n</i></span>. Suppose, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub> = <i>a</i><sub class="lower-index"><i>i</i></sub> - <i>b</i><sub class="lower-index"><i>i</i> + <i>j</i></sub></span>. Then <span class="tex-span"><i>f</i>(<i>j</i>) = |<i>c</i><sub class="lower-index">1</sub> - <i>c</i><sub class="lower-index">2</sub> + <i>c</i><sub class="lower-index">3</sub> - <i>c</i><sub class="lower-index">4</sub>... <i>c</i><sub class="lower-index"><i>n</i></sub>|</span>. More formally, <img align="middle" class="tex-formula" src="file://MvfOp5Ox.png" style="max-width: 100.0%;max-height: 100.0%;">. </p><p>Dr. Evil wants Mahmoud and Ehab to calculate the minimum value of this function over all valid <span class="tex-span"><i>j</i></span>. They found it a bit easy, so Dr. Evil made their task harder. He will give them <span class="tex-span"><i>q</i></span> update queries. During each update they should add an integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> to all elements in <span class="tex-span"><i>a</i></span> in range <span class="tex-span">[<i>l</i><sub class="lower-index"><i>i</i></sub>;<i>r</i><sub class="lower-index"><i>i</i></sub>]</span> i.e. they should add <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>a</i><sub class="lower-index"><i>l</i><sub class="lower-index"><i>i</i></sub></sub>, <i>a</i><sub class="lower-index"><i>l</i><sub class="lower-index"><i>i</i></sub> + 1</sub>, ... , <i>a</i><sub class="lower-index"><i>r</i><sub class="lower-index"><i>i</i></sub></sub></span> and then they should calculate the minimum value of <span class="tex-span"><i>f</i>(<i>j</i>)</span> for all valid <span class="tex-span"><i>j</i></span>.</p><p>Please help Mahmoud and Ehab.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i>, <i>m</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— number of elements in <span class="tex-span"><i>a</i></span>, number of elements in <span class="tex-span"><i>b</i></span> and number of queries, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— elements of <span class="tex-span"><i>a</i></span>.</p><p>The third line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span>. (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— elements of <span class="tex-span"><i>b</i></span>.</p><p>Then <span class="tex-span"><i>q</i></span> lines follow describing the queries. Each of them contains three integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— range to be updated and added value.</p></div><div class="output-specification"><p>The first line should contain the minimum value of the function <span class="tex-span"><i>f</i></span> before any update.</p><p>Then output <span class="tex-span"><i>q</i></span> lines, the <span class="tex-span"><i>i</i></span>-th of them should contain the minimum value of the function <span class="tex-span"><i>f</i></span> after performing the <span class="tex-span"><i>i</i></span>-th update .</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i>, <i>m</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— number of elements in <span class="tex-span"><i>a</i></span>, number of elements in <span class="tex-span"><i>b</i></span> and number of queries, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— elements of <span class="tex-span"><i>a</i></span>.</p><p>The third line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span>. (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— elements of <span class="tex-span"><i>b</i></span>.</p><p>Then <span class="tex-span"><i>q</i></span> lines follow describing the queries. Each of them contains three integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— range to be updated and added value.</p>

## Output

<p>The first line should contain the minimum value of the function <span class="tex-span"><i>f</i></span> before any update.</p><p>Then output <span class="tex-span"><i>q</i></span> lines, the <span class="tex-span"><i>i</i></span>-th of them should contain the minimum value of the function <span class="tex-span"><i>f</i></span> after performing the <span class="tex-span"><i>i</i></span>-th update .</p>





```input1
5 6 3
1 2 3 4 5
1 2 3 4 5 6
1 1 10
1 1 -9
1 5 -1

```




```output1
0
9
0
0

```



## Note

<p>For the first example before any updates it's optimal to choose <span class="tex-span"><i>j</i> = 0</span>, <span class="tex-span"><i>f</i>(0) = |(1 - 1) - (2 - 2) + (3 - 3) - (4 - 4) + (5 - 5)| = |0| = 0</span>.</p><p>After the first update <span class="tex-span"><i>a</i></span> becomes <span class="tex-span">{11, 2, 3, 4, 5}</span> and it's optimal to choose <span class="tex-span"><i>j</i> = 1</span>, <span class="tex-span"><i>f</i>(1) = |(11 - 2) - (2 - 3) + (3 - 4) - (4 - 5) + (5 - 6) = |9| = 9</span>.</p><p>After the second update <span class="tex-span"><i>a</i></span> becomes <span class="tex-span">{2, 2, 3, 4, 5}</span> and it's optimal to choose <span class="tex-span"><i>j</i> = 1</span>, <span class="tex-span"><i>f</i>(1) = |(2 - 2) - (2 - 3) + (3 - 4) - (4 - 5) + (5 - 6)| = |0| = 0</span>.</p><p>After the third update <span class="tex-span"><i>a</i></span> becomes <span class="tex-span">{1, 1, 2, 3, 4}</span> and it's optimal to choose <span class="tex-span"><i>j</i> = 0</span>, <span class="tex-span"><i>f</i>(0) = |(1 - 1) - (1 - 2) + (2 - 3) - (3 - 4) + (4 - 5)| = |0| = 0</span>.</p>