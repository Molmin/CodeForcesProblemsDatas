## Description

<div><p>The following problem is well-known: given integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>, calculate</p><center> <img align="middle" class="tex-formula" src="file://yVfiujlc.png" style="max-width: 100.0%;max-height: 100.0%;">, </center><p>where <span class="tex-span">2<sup class="upper-index"><i>n</i></sup> = 2·2·...·2</span> (<span class="tex-span"><i>n</i></span> factors), and <img align="middle" class="tex-formula" src="file://UqoYs6tf.png" style="max-width: 100.0%;max-height: 100.0%;"> denotes the remainder of division of <span class="tex-span"><i>x</i></span> by <span class="tex-span"><i>y</i></span>.</p><p>You are asked to solve the "reverse" problem. Given integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>, calculate</p><center> <img align="middle" class="tex-formula" src="file://tAexDW9x.png" style="max-width: 100.0%;max-height: 100.0%;">. </center></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">8</sup></span>).</p><p>The second line contains a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">8</sup></span>).</p></div><div class="output-specification"><p>Output a single integer&nbsp;— the value of <img align="middle" class="tex-formula" src="file://HrI0GzPV.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">8</sup></span>).</p><p>The second line contains a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">8</sup></span>).</p>

## Output

<p>Output a single integer&nbsp;— the value of <img align="middle" class="tex-formula" src="file://HrI0GzPV.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
4
42

```




```input2
1
58

```




```input3
98765432
23456789

```




```output1
10

```




```output2
0

```




```output3
23456789

```



## Note

<p>In the first example, the remainder of division of 42 by <span class="tex-span">2<sup class="upper-index">4</sup> = 16</span> is equal to 10.</p><p>In the second example, 58 is divisible by <span class="tex-span">2<sup class="upper-index">1</sup> = 2</span> without remainder, and the answer is 0.</p>
