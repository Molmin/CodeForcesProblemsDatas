## Description

<div><p>Let's assume that we are given a matrix <span class="tex-span"><i>b</i></span> of size <span class="tex-span"><i>x</i> × <i>y</i></span>, let's determine the operation of mirroring matrix <span class="tex-span"><i>b</i></span>. The mirroring of matrix <span class="tex-span"><i>b</i></span> is a <span class="tex-span">2<i>x</i> × <i>y</i></span> matrix <span class="tex-span"><i>c</i></span> which has the following properties:</p><ul> <li> the upper half of matrix <span class="tex-span"><i>c</i></span> (rows with numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>x</i></span>) exactly matches <span class="tex-span"><i>b</i></span>; </li><li> the lower half of matrix <span class="tex-span"><i>c</i></span> (rows with numbers from <span class="tex-span"><i>x</i> + 1</span> to <span class="tex-span">2<i>x</i></span>) is symmetric to the upper one; the symmetry line is the line that separates two halves (the line that goes in the middle, between rows <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>x</i> + 1</span>). </li></ul><p>Sereja has an <span class="tex-span"><i>n</i> × <i>m</i></span> matrix <span class="tex-span"><i>a</i></span>. He wants to find such matrix <span class="tex-span"><i>b</i></span>, that it can be transformed into matrix <span class="tex-span"><i>a</i></span>, if we'll perform on it <span class="tex-font-style-bf">several</span> (possibly zero) mirrorings. What minimum number of rows can such matrix contain?</p></div><div class="input-specification"><p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 100)</span>. Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> integers — the elements of matrix <span class="tex-span"><i>a</i></span>. The <span class="tex-span"><i>i</i></span>-th line contains integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>1</sub>, <i>a</i><sub class="lower-index"><i>i</i>2</sub>, ..., <i>a</i><sub class="lower-index"><i>im</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ 1)</span> — the <span class="tex-span"><i>i</i></span>-th row of the matrix <span class="tex-span"><i>a</i></span>.</p></div><div class="output-specification"><p>In the single line, print the answer to the problem — the minimum number of rows of matrix <span class="tex-span"><i>b</i></span>.</p></div>

## Input

<p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 100)</span>. Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> integers — the elements of matrix <span class="tex-span"><i>a</i></span>. The <span class="tex-span"><i>i</i></span>-th line contains integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>1</sub>, <i>a</i><sub class="lower-index"><i>i</i>2</sub>, ..., <i>a</i><sub class="lower-index"><i>im</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ 1)</span> — the <span class="tex-span"><i>i</i></span>-th row of the matrix <span class="tex-span"><i>a</i></span>.</p>

## Output

<p>In the single line, print the answer to the problem — the minimum number of rows of matrix <span class="tex-span"><i>b</i></span>.</p>





```input1
4 3
0 0 1
1 1 0
1 1 0
0 0 1

```




```input2
3 3
0 0 0
0 0 0
0 0 0

```




```input3
8 1
0
1
1
0
0
1
1
0

```




```output1
2

```




```output2
3

```




```output3
2

```



## Note

<p>In the first test sample the answer is a <span class="tex-span">2 × 3</span> matrix <span class="tex-span"><i>b</i></span>:</p><pre class="verbatim"><br>001<br>110<br></pre><p>If we perform a mirroring operation with this matrix, we get the matrix <span class="tex-span"><i>a</i></span> that is given in the input:</p><pre class="verbatim"><br>001<br>110<br>110<br>001<br></pre>
