## Description

<div><p>Little Chris is a huge fan of linear algebra. This time he has been given a homework about the <span class="tex-font-style-underline">unusual square</span> of a square matrix.</p><p>The <span class="tex-font-style-underline">dot product</span> of two integer number vectors <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> of size <span class="tex-span"><i>n</i></span> is the sum of the products of the corresponding components of the vectors. The <span class="tex-font-style-underline">unusual square</span> of an <span class="tex-span"><i>n</i> × <i>n</i></span> square matrix <span class="tex-span"><i>A</i></span> is defined as the sum of <span class="tex-span"><i>n</i></span> dot products. The <span class="tex-span"><i>i</i></span>-th of them is the dot product of the <span class="tex-span"><i>i</i></span>-th row vector and the <span class="tex-span"><i>i</i></span>-th column vector in the matrix <span class="tex-span"><i>A</i></span>.</p><p>Fortunately for Chris, he has to work only in <span class="tex-span"><i>GF</i>(2)</span>! This means that all operations (addition, multiplication) are calculated modulo 2. In fact, the matrix <span class="tex-span"><i>A</i></span> is binary: each element of <span class="tex-span"><i>A</i></span> is either 0 or 1. For example, consider the following matrix <span class="tex-span"><i>A</i></span>:</p><center> <img class="tex-graphics" src="file://K0Py1lqB.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The unusual square of <span class="tex-span"><i>A</i></span> is equal to <span class="tex-span">(1·1 + 1·0 + 1·1) + (0·1 + 1·1 + 1·0) + (1·1 + 0·1 + 0·0) = 0 + 1 + 1 = 0</span>.</p><p>However, there is much more to the homework. Chris has to process <span class="tex-span"><i>q</i></span> queries; each query can be one of the following: </p><ol> <li> given a row index <span class="tex-span"><i>i</i></span>, flip all the values in the <span class="tex-span"><i>i</i></span>-th row in <span class="tex-span"><i>A</i></span>; </li><li> given a column index <span class="tex-span"><i>i</i></span>, flip all the values in the <span class="tex-span"><i>i</i></span>-th column in <span class="tex-span"><i>A</i></span>; </li><li> find the unusual square of <span class="tex-span"><i>A</i></span>. </li></ol><p>To flip a bit value <span class="tex-span"><i>w</i></span> means to change it to <span class="tex-span">1 - <i>w</i></span>, i.e., 1 changes to 0 and 0 changes to 1.</p><p>Given the initial matrix <span class="tex-span"><i>A</i></span>, output the answers for each query of the third type! Can you solve Chris's homework?</p></div><div class="input-specification"><p>The first line of input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>), the number of rows and the number of columns in the matrix <span class="tex-span"><i>A</i></span>. The next <span class="tex-span"><i>n</i></span> lines describe the matrix: the <span class="tex-span"><i>i</i></span>-th line contains <span class="tex-span"><i>n</i></span> space-separated bits and describes the <span class="tex-span"><i>i</i></span>-th row of <span class="tex-span"><i>A</i></span>. The <span class="tex-span"><i>j</i></span>-th number of the <span class="tex-span"><i>i</i></span>-th line <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ 1</span>) is the element on the intersection of the <span class="tex-span"><i>i</i></span>-th row and the <span class="tex-span"><i>j</i></span>-th column of <span class="tex-span"><i>A</i></span>.</p><p>The next line of input contains an integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">6</sup></span>), the number of queries. Each of the next <span class="tex-span"><i>q</i></span> lines describes a single query, which can be one of the following: </p><ul> <li> 1 <span class="tex-span"><i>i</i></span> — flip the values of the <span class="tex-span"><i>i</i></span>-th row; </li><li> 2 <span class="tex-span"><i>i</i></span> — flip the values of the <span class="tex-span"><i>i</i></span>-th column; </li><li> 3 — output the unusual square of <span class="tex-span"><i>A</i></span>. </li></ul><p><span class="tex-font-style-bf">Note</span>: since the size of the input and output could be very large, don't use slow output techniques in your language. For example, do not use input and output streams (cin, cout) in C++.</p></div><div class="output-specification"><p>Let the number of the 3rd type queries in the input be <span class="tex-span"><i>m</i></span>. Output a single string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>m</i></span>, where the <span class="tex-span"><i>i</i></span>-th symbol of <span class="tex-span"><i>s</i></span> is the value of the unusual square of <span class="tex-span"><i>A</i></span> for the <span class="tex-span"><i>i</i></span>-th query of the 3rd type as it appears in the input.</p></div>

## Input

<p>The first line of input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>), the number of rows and the number of columns in the matrix <span class="tex-span"><i>A</i></span>. The next <span class="tex-span"><i>n</i></span> lines describe the matrix: the <span class="tex-span"><i>i</i></span>-th line contains <span class="tex-span"><i>n</i></span> space-separated bits and describes the <span class="tex-span"><i>i</i></span>-th row of <span class="tex-span"><i>A</i></span>. The <span class="tex-span"><i>j</i></span>-th number of the <span class="tex-span"><i>i</i></span>-th line <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ 1</span>) is the element on the intersection of the <span class="tex-span"><i>i</i></span>-th row and the <span class="tex-span"><i>j</i></span>-th column of <span class="tex-span"><i>A</i></span>.</p><p>The next line of input contains an integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">6</sup></span>), the number of queries. Each of the next <span class="tex-span"><i>q</i></span> lines describes a single query, which can be one of the following: </p><ul> <li> 1 <span class="tex-span"><i>i</i></span> — flip the values of the <span class="tex-span"><i>i</i></span>-th row; </li><li> 2 <span class="tex-span"><i>i</i></span> — flip the values of the <span class="tex-span"><i>i</i></span>-th column; </li><li> 3 — output the unusual square of <span class="tex-span"><i>A</i></span>. </li></ul><p><span class="tex-font-style-bf">Note</span>: since the size of the input and output could be very large, don't use slow output techniques in your language. For example, do not use input and output streams (cin, cout) in C++.</p>

## Output

<p>Let the number of the 3rd type queries in the input be <span class="tex-span"><i>m</i></span>. Output a single string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>m</i></span>, where the <span class="tex-span"><i>i</i></span>-th symbol of <span class="tex-span"><i>s</i></span> is the value of the unusual square of <span class="tex-span"><i>A</i></span> for the <span class="tex-span"><i>i</i></span>-th query of the 3rd type as it appears in the input.</p>





```input1
3
1 1 1
0 1 1
1 0 0
12
3
2 3
3
2 2
2 2
1 3
3
3
1 2
2 1
1 1
3

```




```output1
01001

```


