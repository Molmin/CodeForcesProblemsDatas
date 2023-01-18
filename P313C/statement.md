## Description

<div><p>Ilya is a very good-natured lion. He likes maths. Of all mathematical objects, his favourite one is matrices. Now he's faced a complicated matrix problem he needs to solve.</p><p>He's got a square <span class="tex-span">2<sup class="upper-index"><i>n</i></sup> × 2<sup class="upper-index"><i>n</i></sup></span>-sized matrix and <span class="tex-span">4<sup class="upper-index"><i>n</i></sup></span> integers. You need to arrange all these numbers in the matrix (put each number in a single individual cell) so that the <span class="tex-font-style-it">beauty</span> of the resulting matrix with numbers is maximum.</p><p>The <span class="tex-font-style-it">beauty</span> of a <span class="tex-span">2<sup class="upper-index"><i>n</i></sup> × 2<sup class="upper-index"><i>n</i></sup></span>-sized matrix is an integer, obtained by the following algorithm:</p><ol> <li> Find the maximum element in the matrix. Let's denote it as <span class="tex-span"><i>m</i></span>. </li><li> If <span class="tex-span"><i>n</i> = 0</span>, then the beauty of the matrix equals <span class="tex-span"><i>m</i></span>. Otherwise, a matrix can be split into 4 non-intersecting <span class="tex-span">2<sup class="upper-index"><i>n</i> - 1</sup> × 2<sup class="upper-index"><i>n</i> - 1</sup></span>-sized submatrices, then the beauty of the matrix equals the sum of number <span class="tex-span"><i>m</i></span> and other four beauties of the described submatrices. </li></ol><p>As you can see, the algorithm is recursive.</p><p>Help Ilya, solve the problem and print the resulting maximum beauty of the matrix.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span">4<sup class="upper-index"><i>n</i></sup></span> <span class="tex-span">(1 ≤ 4<sup class="upper-index"><i>n</i></sup> ≤ 2·10<sup class="upper-index">6</sup>)</span>. The next line contains <span class="tex-span">4<sup class="upper-index"><i>n</i></sup></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — the numbers you need to arrange in the <span class="tex-span">2<sup class="upper-index"><i>n</i></sup> × 2<sup class="upper-index"><i>n</i></sup></span>-sized matrix.</p></div><div class="output-specification"><p>On a single line print the maximum value of the beauty of the described matrix.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains integer <span class="tex-span">4<sup class="upper-index"><i>n</i></sup></span> <span class="tex-span">(1 ≤ 4<sup class="upper-index"><i>n</i></sup> ≤ 2·10<sup class="upper-index">6</sup>)</span>. The next line contains <span class="tex-span">4<sup class="upper-index"><i>n</i></sup></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — the numbers you need to arrange in the <span class="tex-span">2<sup class="upper-index"><i>n</i></sup> × 2<sup class="upper-index"><i>n</i></sup></span>-sized matrix.</p>

## Output

<p>On a single line print the maximum value of the beauty of the described matrix.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
1
13

```




```input2
4
1 2 3 4

```




```output1
13

```




```output2
14

```



## Note

<p>Consider the second sample. You need to arrange the numbers in the matrix as follows:</p><pre class="verbatim"><br>1 2<br>3 4<br></pre><p>Then the beauty of the matrix will equal: 4 + 1 + 2 + 3 + 4 = 14.</p>
