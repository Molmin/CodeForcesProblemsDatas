## Description

<div><p>The <span class="tex-font-style-it">determinant</span> of a matrix <span class="tex-span">2 × 2</span> is defined as follows:</p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://t3BDsr5b.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>A matrix is called <span class="tex-font-style-it">degenerate</span> if its determinant is equal to zero. </p><p>The <span class="tex-font-style-it">norm</span> <span class="tex-span">||<i>A</i>||</span> of a matrix <span class="tex-span"><i>A</i></span> is defined as a maximum of absolute values of its elements.</p><p>You are given a matrix <img align="middle" class="tex-formula" src="file://TpZBCVGb.png" style="max-width: 100.0%;max-height: 100.0%;">. Consider any degenerate matrix <span class="tex-span"><i>B</i></span> such that norm <span class="tex-span">||<i>A</i> - <i>B</i>||</span> is minimum possible. Determine <span class="tex-span">||<i>A</i> - <i>B</i>||</span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">|<i>a</i>|, |<i>b</i>| ≤ 10<sup class="upper-index">9</sup></span>), the elements of the first row of matrix <span class="tex-span"><i>A</i></span>. </p><p>The second line contains two integers <span class="tex-span"><i>c</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">|<i>c</i>|, |<i>d</i>| ≤ 10<sup class="upper-index">9</sup></span>) the elements of the second row of matrix <span class="tex-span"><i>A</i></span>.</p></div><div class="output-specification"><p>Output a single real number, the minimum possible value of <span class="tex-span">||<i>A</i> - <i>B</i>||</span>. Your answer is considered to be correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">|<i>a</i>|, |<i>b</i>| ≤ 10<sup class="upper-index">9</sup></span>), the elements of the first row of matrix <span class="tex-span"><i>A</i></span>. </p><p>The second line contains two integers <span class="tex-span"><i>c</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">|<i>c</i>|, |<i>d</i>| ≤ 10<sup class="upper-index">9</sup></span>) the elements of the second row of matrix <span class="tex-span"><i>A</i></span>.</p>

## Output

<p>Output a single real number, the minimum possible value of <span class="tex-span">||<i>A</i> - <i>B</i>||</span>. Your answer is considered to be correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p>





```input1
1 2
3 4

```




```input2
1 0
0 1

```




```output1
0.2000000000

```




```output2
0.5000000000

```



## Note

<p>In the first sample matrix <span class="tex-span"><i>B</i></span> is <img align="middle" class="tex-formula" src="file://Ho0L1awX.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>In the second sample matrix <span class="tex-span"><i>B</i></span> is <img align="middle" class="tex-formula" src="file://6jclYzvg.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
