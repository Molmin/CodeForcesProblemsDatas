## Description

<div><p>You are given a multiset <span class="tex-span"><i>S</i></span> consisting of positive integers (initially empty). There are two kind of queries: </p><ol> <li> Add a positive integer to <span class="tex-span"><i>S</i></span>, the newly added integer is not less than any number in it. </li><li> Find a subset <span class="tex-span"><i>s</i></span> of the set <span class="tex-span"><i>S</i></span> such that the value <img align="middle" class="tex-formula" src="file://ngJm9hIP.png" style="max-width: 100.0%;max-height: 100.0%;"> is maximum possible. Here <span class="tex-span"><i>max</i>(<i>s</i>)</span> means maximum value of elements in <span class="tex-span"><i>s</i></span>, <img align="middle" class="tex-formula" src="file://Tz91LTEc.png" style="max-width: 100.0%;max-height: 100.0%;">&nbsp;— the average value of numbers in <span class="tex-span"><i>s</i></span>. Output this maximum possible value of <img align="middle" class="tex-formula" src="file://Db9mOIcx.png" style="max-width: 100.0%;max-height: 100.0%;">. </li></ol></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>Q</i></span> (<span class="tex-span">1 ≤ <i>Q</i> ≤ 5·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of queries.</p><p>Each of the next <span class="tex-span"><i>Q</i></span> lines contains a description of query. For queries of type <span class="tex-span">1</span> two integers <span class="tex-span">1</span> and <span class="tex-span"><i>x</i></span> are given, where <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>) is a number that you should add to <span class="tex-span"><i>S</i></span>. It's guaranteed that <span class="tex-span"><i>x</i></span> is not less than any number in <span class="tex-span"><i>S</i></span>. For queries of type <span class="tex-span">2</span>, a single integer <span class="tex-span">2</span> is given.</p><p>It's guaranteed that the first query has type <span class="tex-span">1</span>, i.&nbsp;e. <span class="tex-span"><i>S</i></span> is not empty when a query of type <span class="tex-span">2</span> comes.</p></div><div class="output-specification"><p>Output the answer for each query of the second type in the order these queries are given in input. Each number should be printed in separate line.</p><p>Your answer is considered correct, if each of your answers has absolute or relative error not greater than <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p><p>Formally, let your answer be <span class="tex-span"><i>a</i></span>, and the jury's answer be <span class="tex-span"><i>b</i></span>. Your answer is considered correct if <img align="middle" class="tex-formula" src="file://mvCGlBw4.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>Q</i></span> (<span class="tex-span">1 ≤ <i>Q</i> ≤ 5·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of queries.</p><p>Each of the next <span class="tex-span"><i>Q</i></span> lines contains a description of query. For queries of type <span class="tex-span">1</span> two integers <span class="tex-span">1</span> and <span class="tex-span"><i>x</i></span> are given, where <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>) is a number that you should add to <span class="tex-span"><i>S</i></span>. It's guaranteed that <span class="tex-span"><i>x</i></span> is not less than any number in <span class="tex-span"><i>S</i></span>. For queries of type <span class="tex-span">2</span>, a single integer <span class="tex-span">2</span> is given.</p><p>It's guaranteed that the first query has type <span class="tex-span">1</span>, i.&nbsp;e. <span class="tex-span"><i>S</i></span> is not empty when a query of type <span class="tex-span">2</span> comes.</p>

## Output

<p>Output the answer for each query of the second type in the order these queries are given in input. Each number should be printed in separate line.</p><p>Your answer is considered correct, if each of your answers has absolute or relative error not greater than <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p><p>Formally, let your answer be <span class="tex-span"><i>a</i></span>, and the jury's answer be <span class="tex-span"><i>b</i></span>. Your answer is considered correct if <img align="middle" class="tex-formula" src="file://mvCGlBw4.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
6
1 3
2
1 4
2
1 8
2

```




```input2
4
1 1
1 4
1 5
2

```




```output1
0.0000000000
0.5000000000
3.0000000000

```




```output2
2.0000000000

```


