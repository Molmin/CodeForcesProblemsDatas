## Description

<div><p>Maxim loves to fill in a matrix in a special manner. Here is a pseudocode of filling in a matrix of size <span class="tex-span">(<i>m</i> + 1) × (<i>m</i> + 1)</span>:</p><p><img class="tex-graphics" src="file://ANUZcr39.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Maxim asks you to count, how many numbers <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ <i>n</i>)</span> are there, such that the sum of values in the cells in the row number <span class="tex-span"><i>m</i> + 1</span> of the resulting matrix equals <span class="tex-span"><i>t</i></span>.</p><p>Expression (<span class="tex-span"><i>x</i></span> <span class="tex-span"><i>xor</i></span> <span class="tex-span"><i>y</i></span>) means applying the operation of bitwise excluding "OR" to numbers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>. The given operation exists in all modern programming languages. For example, in languages <span class="tex-font-style-it">C++</span> and <span class="tex-font-style-it">Java</span> it is represented by character "<span class="tex-font-style-tt">^</span>", in <span class="tex-font-style-it">Pascal</span> — by "<span class="tex-font-style-tt">xor</span>".</p></div><div class="input-specification"><p>A single line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>t</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>t</i> ≤ 10<sup class="upper-index">12</sup>, <i>t</i> ≤ <i>n</i> + 1)</span>.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in <span class="tex-font-style-it">C++</span>. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div><div class="output-specification"><p>In a single line print a single integer — the answer to the problem. </p></div>

## Input

<p>A single line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>t</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>t</i> ≤ 10<sup class="upper-index">12</sup>, <i>t</i> ≤ <i>n</i> + 1)</span>.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in <span class="tex-font-style-it">C++</span>. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>

## Output

<p>In a single line print a single integer — the answer to the problem. </p>





```input1
1 1

```




```input2
3 2

```




```input3
3 3

```




```input4
1000000000000 1048576

```




```output1
1

```




```output2
1

```




```output3
0

```




```output4
118606527258

```


