## Description

<div><p>Little Petya is now fond of data compression algorithms. He has already studied <span class="tex-font-style-it">gz</span>, <span class="tex-font-style-it">bz</span>, <span class="tex-font-style-it">zip</span> algorithms and many others. Inspired by the new knowledge, Petya is now developing the new compression algorithm which he wants to name <span class="tex-font-style-it">dis</span>.</p><p>Petya decided to compress tables. He is given a table <span class="tex-span"><i>a</i></span> consisting of <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>m</i></span> columns that is filled with positive integers. He wants to build the table <span class="tex-span"><i>a</i>'</span> consisting of positive integers such that the relative order of the elements in each row and each column remains the same. That is, if in some row <span class="tex-span"><i>i</i></span> of the initial table <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> &lt; <i>a</i><sub class="lower-index"><i>i</i>, <i>k</i></sub></span>, then in the resulting table <span class="tex-span"><i>a</i>'<sub class="lower-index"><i>i</i>, <i>j</i></sub> &lt; <i>a</i>'<sub class="lower-index"><i>i</i>, <i>k</i></sub></span>, and if <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = <i>a</i><sub class="lower-index"><i>i</i>, <i>k</i></sub></span> then <span class="tex-span"><i>a</i>'<sub class="lower-index"><i>i</i>, <i>j</i></sub> = <i>a</i>'<sub class="lower-index"><i>i</i>, <i>k</i></sub></span>. Similarly, if in some column <span class="tex-span"><i>j</i></span> of the initial table <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> &lt; <i>a</i><sub class="lower-index"><i>p</i>, <i>j</i></sub></span> then in compressed table <span class="tex-span"><i>a</i>'<sub class="lower-index"><i>i</i>, <i>j</i></sub> &lt; <i>a</i>'<sub class="lower-index"><i>p</i>, <i>j</i></sub></span> and if <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = <i>a</i><sub class="lower-index"><i>p</i>, <i>j</i></sub></span> then <span class="tex-span"><i>a</i>'<sub class="lower-index"><i>i</i>, <i>j</i></sub> = <i>a</i>'<sub class="lower-index"><i>p</i>, <i>j</i></sub></span>. </p><p>Because large values require more space to store them, the maximum value in <span class="tex-span"><i>a</i>'</span> should be as small as possible.</p><p>Petya is good in theory, however, he needs your help to implement the algorithm.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<img align="middle" class="tex-formula" src="file://EIGpa7QA.png" style="max-width: 100.0%;max-height: 100.0%;">, the number of rows and the number of columns of the table respectively.</p><p>Each of the following <span class="tex-span"><i>n</i></span> rows contain <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> that are the values in the table.</p></div><div class="output-specification"><p>Output the compressed table in form of <span class="tex-span"><i>n</i></span> lines each containing <span class="tex-span"><i>m</i></span> integers.</p><p>If there exist several answers such that the maximum number in the compressed table is minimum possible, you are allowed to output any of them.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<img align="middle" class="tex-formula" src="file://EIGpa7QA.png" style="max-width: 100.0%;max-height: 100.0%;">, the number of rows and the number of columns of the table respectively.</p><p>Each of the following <span class="tex-span"><i>n</i></span> rows contain <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> that are the values in the table.</p>

## Output

<p>Output the compressed table in form of <span class="tex-span"><i>n</i></span> lines each containing <span class="tex-span"><i>m</i></span> integers.</p><p>If there exist several answers such that the maximum number in the compressed table is minimum possible, you are allowed to output any of them.</p>





```input1
2 2
1 2
3 4

```




```input2
4 3
20 10 30
50 40 30
50 60 70
90 80 70

```




```output1
1 2
2 3

```




```output2
2 1 3
5 4 3
5 6 7
9 8 7

```



## Note

<p>In the first sample test, despite the fact <span class="tex-span"><i>a</i><sub class="lower-index">1, 2</sub> ≠ <i>a</i><sub class="lower-index">21</sub></span>, they are not located in the same row or column so they may become equal after the compression.</p>
