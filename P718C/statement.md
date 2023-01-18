## Description

<div><p>Sasha has an array of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. You have to perform <span class="tex-span"><i>m</i></span> queries. There might be queries of two types:</p><ol> <li> <span class="tex-font-style-tt">1 l r x</span>&nbsp;— increase all integers on the segment from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span> by values <span class="tex-span"><i>x</i></span>; </li><li> <span class="tex-font-style-tt">2 l r</span>&nbsp;— find <img align="middle" class="tex-formula" src="file://OnsFqn0v.png" style="max-width: 100.0%;max-height: 100.0%;">, where <span class="tex-span"><i>f</i>(<i>x</i>)</span> is the <span class="tex-span"><i>x</i></span>-th Fibonacci number. As this number may be large, you only have to find it modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>. </li></ol><p>In this problem we define Fibonacci numbers as follows: <span class="tex-span"><i>f</i>(1) = 1</span>, <span class="tex-span"><i>f</i>(2) = 1</span>, <span class="tex-span"><i>f</i>(<i>x</i>) = <i>f</i>(<i>x</i> - 1) + <i>f</i>(<i>x</i> - 2)</span> for all <span class="tex-span"><i>x</i> &gt; 2</span>.</p><p>Sasha is a very talented boy and he managed to perform all queries in five seconds. Will you be able to write the program that performs as well as Sasha?</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 100 000</span>)&nbsp;— the number of elements in the array and the number of queries respectively.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>Then follow <span class="tex-span"><i>m</i></span> lines with queries descriptions. Each of them contains integers <span class="tex-span"><i>tp</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and may be <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>tp</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>, <span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). Here <span class="tex-span"><i>tp</i><sub class="lower-index"><i>i</i></sub> = 1</span> corresponds to the queries of the first type and <span class="tex-span"><i>tp</i><sub class="lower-index"><i>i</i></sub></span> corresponds to the queries of the second type.</p><p>It's guaranteed that the input will contains at least one query of the second type.</p></div><div class="output-specification"><p>For each query of the second type print the answer modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 100 000</span>)&nbsp;— the number of elements in the array and the number of queries respectively.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>Then follow <span class="tex-span"><i>m</i></span> lines with queries descriptions. Each of them contains integers <span class="tex-span"><i>tp</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and may be <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>tp</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>, <span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). Here <span class="tex-span"><i>tp</i><sub class="lower-index"><i>i</i></sub> = 1</span> corresponds to the queries of the first type and <span class="tex-span"><i>tp</i><sub class="lower-index"><i>i</i></sub></span> corresponds to the queries of the second type.</p><p>It's guaranteed that the input will contains at least one query of the second type.</p>

## Output

<p>For each query of the second type print the answer modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
5 4
1 1 2 1 1
2 1 5
1 2 4 2
2 2 4
2 1 5

```




```output1
5
7
9

```



## Note

<p>Initially, array <span class="tex-span"><i>a</i></span> is equal to <span class="tex-span">1</span>, <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">1</span>, <span class="tex-span">1</span>.</p><p>The answer for the first query of the second type is <span class="tex-span"><i>f</i>(1) + <i>f</i>(1) + <i>f</i>(2) + <i>f</i>(1) + <i>f</i>(1) = 1 + 1 + 1 + 1 + 1 = 5</span>. </p><p>After the query <span class="tex-font-style-tt">1 2 4 2</span> array <span class="tex-span"><i>a</i></span> is equal to <span class="tex-span">1</span>, <span class="tex-span">3</span>, <span class="tex-span">4</span>, <span class="tex-span">3</span>, <span class="tex-span">1</span>.</p><p>The answer for the second query of the second type is <span class="tex-span"><i>f</i>(3) + <i>f</i>(4) + <i>f</i>(3) = 2 + 3 + 2 = 7</span>.</p><p>The answer for the third query of the second type is <span class="tex-span"><i>f</i>(1) + <i>f</i>(3) + <i>f</i>(4) + <i>f</i>(3) + <i>f</i>(1) = 1 + 2 + 3 + 2 + 1 = 9</span>.</p>
