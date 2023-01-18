## Description

<div><p>Iahub does not like background stories, so he'll tell you exactly what this problem asks you for.</p><p>You are given a matrix <span class="tex-span"><i>a</i></span> with <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>n</i></span> columns. Initially, all values of the matrix are zeros. Both rows and columns are 1-based, that is rows are numbered 1, 2, ..., <span class="tex-span"><i>n</i></span> and columns are numbered 1, 2, ..., <span class="tex-span"><i>n</i></span>. Let's denote an element on the <span class="tex-span"><i>i</i></span>-th row and <span class="tex-span"><i>j</i></span>-th column as <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span>.</p><p>We will call a submatrix <span class="tex-span">(<i>x</i><sub class="lower-index">0</sub>, <i>y</i><sub class="lower-index">0</sub>, <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> such elements <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> for which two inequalities hold: <span class="tex-span"><i>x</i><sub class="lower-index">0</sub> ≤ <i>i</i> ≤ <i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">0</sub> ≤ <i>j</i> ≤ <i>y</i><sub class="lower-index">1</sub></span>.</p><p>Write a program to perform two following operations:</p><ol> <li> Query(<span class="tex-span"><i>x</i><sub class="lower-index">0</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">0</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>): print the xor sum of the elements of the submatrix <span class="tex-span">(<i>x</i><sub class="lower-index">0</sub>, <i>y</i><sub class="lower-index">0</sub>, <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span>. </li><li> Update(<span class="tex-span"><i>x</i><sub class="lower-index">0</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">0</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>v</i></span>): each element from submatrix <span class="tex-span">(<i>x</i><sub class="lower-index">0</sub>, <i>y</i><sub class="lower-index">0</sub>, <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> gets xor-ed by value <span class="tex-span"><i>v</i></span>. </li></ol></div><div class="input-specification"><p>The first line contains two integers: <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>). The number <span class="tex-span"><i>m</i></span> represents the number of operations you need to perform. Each of the next <span class="tex-span"><i>m</i></span> lines contains five or six integers, depending on operation type. </p><p>If the <span class="tex-span"><i>i</i></span>-th operation from the input is a query, the first number from <span class="tex-span"><i>i</i></span>-th line will be 1. It will be followed by four integers <span class="tex-span"><i>x</i><sub class="lower-index">0</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">0</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>. If the <span class="tex-span"><i>i</i></span>-th operation is an update, the first number from the <span class="tex-span"><i>i</i></span>-th line will be 2. It will be followed by five integers <span class="tex-span"><i>x</i><sub class="lower-index">0</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">0</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>v</i></span>. </p><p>It is guaranteed that for each update operation, the following inequality holds: <span class="tex-span">0 ≤ <i>v</i> &lt; 2<sup class="upper-index">62</sup></span>. It is guaranteed that for each operation, the following inequalities hold: <span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">0</sub> ≤ <i>x</i><sub class="lower-index">1</sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index">0</sub> ≤ <i>y</i><sub class="lower-index">1</sub> ≤ <i>n</i></span>.</p></div><div class="output-specification"><p>For each query operation, output on a new line the result.</p></div>

## Input

<p>The first line contains two integers: <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>). The number <span class="tex-span"><i>m</i></span> represents the number of operations you need to perform. Each of the next <span class="tex-span"><i>m</i></span> lines contains five or six integers, depending on operation type. </p><p>If the <span class="tex-span"><i>i</i></span>-th operation from the input is a query, the first number from <span class="tex-span"><i>i</i></span>-th line will be 1. It will be followed by four integers <span class="tex-span"><i>x</i><sub class="lower-index">0</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">0</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>. If the <span class="tex-span"><i>i</i></span>-th operation is an update, the first number from the <span class="tex-span"><i>i</i></span>-th line will be 2. It will be followed by five integers <span class="tex-span"><i>x</i><sub class="lower-index">0</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">0</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>v</i></span>. </p><p>It is guaranteed that for each update operation, the following inequality holds: <span class="tex-span">0 ≤ <i>v</i> &lt; 2<sup class="upper-index">62</sup></span>. It is guaranteed that for each operation, the following inequalities hold: <span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">0</sub> ≤ <i>x</i><sub class="lower-index">1</sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index">0</sub> ≤ <i>y</i><sub class="lower-index">1</sub> ≤ <i>n</i></span>.</p>

## Output

<p>For each query operation, output on a new line the result.</p>





```input1
3 5
2 1 1 2 2 1
2 1 3 2 3 2
2 3 1 3 3 3
1 2 2 3 3
1 2 2 3 2

```




```output1
3
2

```



## Note

<p>After the first <span class="tex-span">3</span> operations, the matrix will look like this: </p><pre class="verbatim"><br>1 1 2<br>1 1 2<br>3 3 3<br></pre><p>The fourth operation asks us to compute 1 xor 2 xor 3 xor 3 = 3.</p><p>The fifth operation asks us to compute 1 xor 3 = 2. </p>
