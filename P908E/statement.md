## Description

<div><p>You are given an integer <span class="tex-span"><i>m</i></span>.</p><p>Let <span class="tex-span"><i>M</i> = 2<sup class="upper-index"><i>m</i></sup> - 1</span>.</p><p>You are also given a set of <span class="tex-span"><i>n</i></span> integers denoted as the set <span class="tex-span"><i>T</i></span>. The integers will be provided in base 2 as <span class="tex-span"><i>n</i></span> binary strings of length <span class="tex-span"><i>m</i></span>.</p><p>A set of integers <span class="tex-span"><i>S</i></span> is called "good" if the following hold. </p><ol> <li> If <img align="middle" class="tex-formula" src="file://Qv1JQK9A.png" style="max-width: 100.0%;max-height: 100.0%;">, then <img align="middle" class="tex-formula" src="file://r6VEmAnR.png" style="max-width: 100.0%;max-height: 100.0%;">. </li><li> If <img align="middle" class="tex-formula" src="file://AOAGoCg0.png" style="max-width: 100.0%;max-height: 100.0%;">, then <img align="middle" class="tex-formula" src="file://J3que4Ve.png" style="max-width: 100.0%;max-height: 100.0%;"> </li><li> <img align="middle" class="tex-formula" src="file://2RC1LlCG.png" style="max-width: 100.0%;max-height: 100.0%;"> </li><li> All elements of <span class="tex-span"><i>S</i></span> are less than or equal to <span class="tex-span"><i>M</i></span>. </li></ol><p>Here, <img align="middle" class="tex-formula" src="file://mqbiuEWt.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="file://a17roetM.png" style="max-width: 100.0%;max-height: 100.0%;"> refer to the bitwise XOR and bitwise AND operators, respectively.</p><p>Count the number of good sets <span class="tex-span"><i>S</i></span>, modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line will contain two integers <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 1 000</span>, <span class="tex-span">1 ≤ <i>n</i> ≤ <i>min</i>(2<sup class="upper-index"><i>m</i></sup>, 50)</span>).</p><p>The next <span class="tex-span"><i>n</i></span> lines will contain the elements of <span class="tex-span"><i>T</i></span>. Each line will contain exactly <span class="tex-span"><i>m</i></span> zeros and ones. Elements of <span class="tex-span"><i>T</i></span> will be distinct.</p></div><div class="output-specification"><p>Print a single integer, the number of good sets modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>. </p></div>

## Input

<p>The first line will contain two integers <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 1 000</span>, <span class="tex-span">1 ≤ <i>n</i> ≤ <i>min</i>(2<sup class="upper-index"><i>m</i></sup>, 50)</span>).</p><p>The next <span class="tex-span"><i>n</i></span> lines will contain the elements of <span class="tex-span"><i>T</i></span>. Each line will contain exactly <span class="tex-span"><i>m</i></span> zeros and ones. Elements of <span class="tex-span"><i>T</i></span> will be distinct.</p>

## Output

<p>Print a single integer, the number of good sets modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>. </p>





```input1
5 3
11010
00101
11000

```




```input2
30 2
010101010101010010101010101010
110110110110110011011011011011

```




```output1
4

```




```output2
860616440

```



## Note

<p>An example of a valid set <span class="tex-span"><i>S</i></span> is {00000, 00101, 00010, 00111, 11000, 11010, 11101, 11111}.</p>
