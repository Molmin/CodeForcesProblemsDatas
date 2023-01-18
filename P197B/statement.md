## Description

<div><p>You are given two polynomials:</p><ul> <li> <span class="tex-span"><i>P</i>(<i>x</i>) = <i>a</i><sub class="lower-index">0</sub>·<i>x</i><sup class="upper-index"><i>n</i></sup> + <i>a</i><sub class="lower-index">1</sub>·<i>x</i><sup class="upper-index"><i>n</i> - 1</sup> + ... + <i>a</i><sub class="lower-index"><i>n</i> - 1</sub>·<i>x</i> + <i>a</i><sub class="lower-index"><i>n</i></sub></span> and </li><li> <span class="tex-span"><i>Q</i>(<i>x</i>) = <i>b</i><sub class="lower-index">0</sub>·<i>x</i><sup class="upper-index"><i>m</i></sup> + <i>b</i><sub class="lower-index">1</sub>·<i>x</i><sup class="upper-index"><i>m</i> - 1</sup> + ... + <i>b</i><sub class="lower-index"><i>m</i> - 1</sub>·<i>x</i> + <i>b</i><sub class="lower-index"><i>m</i></sub></span>. </li></ul> <p>Calculate limit <img align="middle" class="tex-formula" src="file://lf52Ois1.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>n</i>, <i>m</i> ≤ 100</span>) — degrees of polynomials <span class="tex-span"><i>P</i>(<i>x</i>)</span> and <span class="tex-span"><i>Q</i>(<i>x</i>)</span> correspondingly.</p><p>The second line contains <span class="tex-span"><i>n</i> + 1</span> space-separated integers — the factors of polynomial <span class="tex-span"><i>P</i>(<i>x</i>)</span>: <span class="tex-span"><i>a</i><sub class="lower-index">0</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">( - 100 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100, <i>a</i><sub class="lower-index">0</sub> ≠ 0)</span>.</p><p>The third line contains <span class="tex-span"><i>m</i> + 1</span> space-separated integers — the factors of polynomial <span class="tex-span"><i>Q</i>(<i>x</i>)</span>: <span class="tex-span"><i>b</i><sub class="lower-index">0</sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span>, ..., <span class="tex-span"><i>b</i><sub class="lower-index"><i>m</i> - 1</sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>m</i></sub></span> <span class="tex-span">( - 100 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 100, <i>b</i><sub class="lower-index">0</sub> ≠ 0)</span>.</p></div><div class="output-specification"><p>If the limit equals <span class="tex-span"> + ∞</span>, print "<span class="tex-font-style-tt">Infinity</span>" (without quotes). If the limit equals <span class="tex-span"> - ∞</span>, print "<span class="tex-font-style-tt">-Infinity</span>" (without the quotes).</p><p>If the value of the limit equals zero, print "<span class="tex-font-style-tt">0/1</span>" (without the quotes).</p><p>Otherwise, print an irreducible fraction — the value of limit <img align="middle" class="tex-formula" src="file://wcL36vFn.png" style="max-width: 100.0%;max-height: 100.0%;">, in the format "<span class="tex-font-style-tt">p/q</span>" (without the quotes), where <span class="tex-span"><i>p</i></span> is the — numerator, <span class="tex-span"><i>q</i></span> <span class="tex-span">(<i>q</i> &gt; 0)</span> is the denominator of the fraction.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>n</i>, <i>m</i> ≤ 100</span>) — degrees of polynomials <span class="tex-span"><i>P</i>(<i>x</i>)</span> and <span class="tex-span"><i>Q</i>(<i>x</i>)</span> correspondingly.</p><p>The second line contains <span class="tex-span"><i>n</i> + 1</span> space-separated integers — the factors of polynomial <span class="tex-span"><i>P</i>(<i>x</i>)</span>: <span class="tex-span"><i>a</i><sub class="lower-index">0</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">( - 100 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100, <i>a</i><sub class="lower-index">0</sub> ≠ 0)</span>.</p><p>The third line contains <span class="tex-span"><i>m</i> + 1</span> space-separated integers — the factors of polynomial <span class="tex-span"><i>Q</i>(<i>x</i>)</span>: <span class="tex-span"><i>b</i><sub class="lower-index">0</sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span>, ..., <span class="tex-span"><i>b</i><sub class="lower-index"><i>m</i> - 1</sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>m</i></sub></span> <span class="tex-span">( - 100 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 100, <i>b</i><sub class="lower-index">0</sub> ≠ 0)</span>.</p>

## Output

<p>If the limit equals <span class="tex-span"> + ∞</span>, print "<span class="tex-font-style-tt">Infinity</span>" (without quotes). If the limit equals <span class="tex-span"> - ∞</span>, print "<span class="tex-font-style-tt">-Infinity</span>" (without the quotes).</p><p>If the value of the limit equals zero, print "<span class="tex-font-style-tt">0/1</span>" (without the quotes).</p><p>Otherwise, print an irreducible fraction — the value of limit <img align="middle" class="tex-formula" src="file://wcL36vFn.png" style="max-width: 100.0%;max-height: 100.0%;">, in the format "<span class="tex-font-style-tt">p/q</span>" (without the quotes), where <span class="tex-span"><i>p</i></span> is the — numerator, <span class="tex-span"><i>q</i></span> <span class="tex-span">(<i>q</i> &gt; 0)</span> is the denominator of the fraction.</p>





```input1
2 1
1 1 1
2 5

```




```input2
1 0
-1 3
2

```




```input3
0 1
1
1 0

```




```input4
2 2
2 1 6
4 5 -7

```




```input5
1 1
9 0
-5 2

```




```output1
Infinity

```




```output2
-Infinity

```




```output3
0/1

```




```output4
1/2

```




```output5
-9/5

```



## Note

<p>Let's consider all samples:</p><ol> <li> <img align="middle" class="tex-formula" src="file://9UOsYluw.png" style="max-width: 100.0%;max-height: 100.0%;"> </li><li> <img align="middle" class="tex-formula" src="file://YZPtGYpU.png" style="max-width: 100.0%;max-height: 100.0%;"> </li><li> <img align="middle" class="tex-formula" src="file://el1gggJD.png" style="max-width: 100.0%;max-height: 100.0%;"> </li><li> <img align="middle" class="tex-formula" src="file://h0QLb4UQ.png" style="max-width: 100.0%;max-height: 100.0%;"> </li><li> <img align="middle" class="tex-formula" src="file://D5EzOAHf.png" style="max-width: 100.0%;max-height: 100.0%;"> </li></ol><p>You can learn more about the definition and properties of limits if you follow the link: <span class="tex-font-style-tt">http://en.wikipedia.org/wiki/Limit_of_a_function</span></p>
