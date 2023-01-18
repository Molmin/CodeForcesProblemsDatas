## Description

<div><p>Limak, a bear, isn't good at handling queries. So, he asks you to do it.</p><p>We say that powers of <span class="tex-span">42</span> (numbers <span class="tex-span">1, 42, 1764, ...</span>) are <span class="tex-font-style-it">bad</span>. Other numbers are <span class="tex-font-style-it">good</span>.</p><p>You are given a sequence of <span class="tex-span"><i>n</i></span> good integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span>. Your task is to handle <span class="tex-span"><i>q</i></span> queries of three types:</p><ol> <li> <span class="tex-font-style-tt">1 i</span>&nbsp;— print <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> in a separate line. </li><li> <span class="tex-font-style-tt">2 a b x</span>&nbsp;— for <img align="middle" class="tex-formula" src="file://qmMYVYRp.png" style="max-width: 100.0%;max-height: 100.0%;"> set <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>x</i></span>. It's guaranteed that <span class="tex-span"><i>x</i></span> is a good number. </li><li> <span class="tex-font-style-tt">3 a b x</span>&nbsp;— for <img align="middle" class="tex-formula" src="file://SgUY7MBe.png" style="max-width: 100.0%;max-height: 100.0%;"> increase <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> by <span class="tex-span"><i>x</i></span>. After this repeat the process while at least one <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is bad. </li></ol><p>You can note that after each query all <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> are good.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>q</i> ≤ 100 000</span>)&nbsp;— the size of Limak's sequence and the number of queries, respectively.</p><p>The second line of the input contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">2 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— initial elements of Limak's sequence. All <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> are good.</p><p>Then, <span class="tex-span"><i>q</i></span> lines follow. The <span class="tex-span"><i>i</i></span>-th of them describes the <span class="tex-span"><i>i</i></span>-th query. The first number in the line is an integer <span class="tex-span"><i>type</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>type</i><sub class="lower-index"><i>i</i></sub> ≤ 3</span>)&nbsp;— the type of the query. There is at least one query of the first type, so the output won't be empty.</p><p>In queries of the second and the third type there is <span class="tex-span">1 ≤ <i>a</i> ≤ <i>b</i> ≤ <i>n</i></span>.</p><p>In queries of the second type an integer <span class="tex-span"><i>x</i></span> (<span class="tex-span">2 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>) is guaranteed to be good.</p><p>In queries of the third type an integer <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>) may be bad.</p></div><div class="output-specification"><p>For each query of the first type, print the answer in a separate line.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>q</i> ≤ 100 000</span>)&nbsp;— the size of Limak's sequence and the number of queries, respectively.</p><p>The second line of the input contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">2 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— initial elements of Limak's sequence. All <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> are good.</p><p>Then, <span class="tex-span"><i>q</i></span> lines follow. The <span class="tex-span"><i>i</i></span>-th of them describes the <span class="tex-span"><i>i</i></span>-th query. The first number in the line is an integer <span class="tex-span"><i>type</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>type</i><sub class="lower-index"><i>i</i></sub> ≤ 3</span>)&nbsp;— the type of the query. There is at least one query of the first type, so the output won't be empty.</p><p>In queries of the second and the third type there is <span class="tex-span">1 ≤ <i>a</i> ≤ <i>b</i> ≤ <i>n</i></span>.</p><p>In queries of the second type an integer <span class="tex-span"><i>x</i></span> (<span class="tex-span">2 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>) is guaranteed to be good.</p><p>In queries of the third type an integer <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>) may be bad.</p>

## Output

<p>For each query of the first type, print the answer in a separate line.</p>





```input1
6 12
40 1700 7 1672 4 1722
3 2 4 42
1 2
1 3
3 2 6 50
1 2
1 4
1 6
2 3 4 41
3 1 5 1
1 1
1 3
1 5

```




```output1
1742
49
1842
1814
1822
43
44
107

```



## Note

<p>After a query <span class="tex-font-style-tt">3 2 4 42</span> the sequence is <span class="tex-span">40, 1742, 49, 1714, 4, 1722</span>.</p><p>After a query <span class="tex-font-style-tt">3 2 6 50</span> the sequence is <span class="tex-span">40, 1842, 149, 1814, 104, 1822</span>.</p><p>After a query <span class="tex-font-style-tt">2 3 4 41</span> the sequence is <span class="tex-span">40, 1842, 41, 41, 104, 1822</span>.</p><p>After a query <span class="tex-font-style-tt">3 1 5 1</span> the sequence is <span class="tex-span">43, 1845, 44, 44, 107, 1822</span>.</p>
