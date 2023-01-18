## Description

<div><p>Little Mishka enjoys programming. Since her birthday has just passed, her friends decided to present her with array of non-negative integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> of <span class="tex-span"><i>n</i></span> elements!</p><p>Mishka loved the array and she instantly decided to determine its beauty value, but she is too little and can't process large arrays. Right because of that she invited you to visit her and asked you to process <span class="tex-span"><i>m</i></span> queries.</p><p>Each query is processed in the following way:</p><ol> <li> Two integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>) are specified&nbsp;— bounds of query segment. </li><li> Integers, presented in array segment <span class="tex-span">[<i>l</i>,  <i>r</i>]</span> (in sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>l</i></sub>, <i>a</i><sub class="lower-index"><i>l</i> + 1</sub>, ..., <i>a</i><sub class="lower-index"><i>r</i></sub></span>) <span class="tex-font-style-bf">even number of times</span>, are written down. </li><li> XOR-sum of written down integers is calculated, and this value is the answer for a query. Formally, if integers written down in point 2 are <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>k</i></sub></span>, then Mishka wants to know the value <img align="middle" class="tex-formula" src="file://pftjwF7y.png" style="max-width: 100.0%;max-height: 100.0%;">, where <img align="middle" class="tex-formula" src="file://Mxhs8xoi.png" style="max-width: 100.0%;max-height: 100.0%;">&nbsp;— operator of exclusive bitwise OR. </li></ol><p>Since only the little bears know the definition of array beauty, all you are to do is to answer each of queries presented.</p></div><div class="input-specification"><p>The first line of the input contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1 000 000</span>)&nbsp;— the number of elements in the array.</p><p>The second line of the input contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— array elements.</p><p>The third line of the input contains single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 1 000 000</span>)&nbsp;— the number of queries.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines describes corresponding query by a pair of integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>)&nbsp;— the bounds of query segment.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> non-negative integers&nbsp;— the answers for the queries in the order they appear in the input.</p></div>

## Input

<p>The first line of the input contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1 000 000</span>)&nbsp;— the number of elements in the array.</p><p>The second line of the input contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— array elements.</p><p>The third line of the input contains single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 1 000 000</span>)&nbsp;— the number of queries.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines describes corresponding query by a pair of integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>)&nbsp;— the bounds of query segment.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> non-negative integers&nbsp;— the answers for the queries in the order they appear in the input.</p>





```input1
3
3 7 8
1
1 3

```




```input2
7
1 2 1 3 3 2 3
5
4 7
4 5
1 3
1 7
1 5

```




```output1
0

```




```output2
0
3
1
3
2

```



## Note

<p>In the second sample:</p><p>There is no integers in the segment of the first query, presented even number of times in the segment&nbsp;— the answer is <span class="tex-span">0</span>.</p><p>In the second query there is only integer <span class="tex-span">3</span> is presented even number of times&nbsp;— the answer is <span class="tex-span">3</span>.</p><p>In the third query only integer <span class="tex-span">1</span> is written down&nbsp;— the answer is <span class="tex-span">1</span>.</p><p>In the fourth query all array elements are considered. Only <span class="tex-span">1</span> and <span class="tex-span">2</span> are presented there even number of times. The answer is <img align="middle" class="tex-formula" src="file://gN0CMuat.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>In the fifth query <span class="tex-span">1</span> and <span class="tex-span">3</span> are written down. The answer is <img align="middle" class="tex-formula" src="file://uFCF8nAF.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
