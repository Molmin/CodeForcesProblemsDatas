## Description

<div><p>Let's consider equation:</p><center class="tex-equation"><span class="tex-span"><i>x</i><sup class="upper-index">2</sup> + <i>s</i>(<i>x</i>)·<i>x</i> - <i>n</i> = 0, </span></center> <p>where <span class="tex-span"><i>x</i>, <i>n</i></span> are positive integers, <span class="tex-span"><i>s</i>(<i>x</i>)</span> is the function, equal to the sum of digits of number <span class="tex-span"><i>x</i></span> in the decimal number system.</p><p>You are given an integer <span class="tex-span"><i>n</i></span>, find the smallest positive integer root of equation <span class="tex-span"><i>x</i></span>, or else determine that there are no such roots.</p></div><div class="input-specification"><p>A single line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup>)</span> — the equation parameter.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier. </p></div><div class="output-specification"><p>Print -1, if the equation doesn't have integer positive roots. Otherwise print such smallest integer <span class="tex-span"><i>x</i></span> <span class="tex-span">(<i>x</i> &gt; 0)</span>, that the equation given in the statement holds.</p></div>

## Input

<p>A single line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup>)</span> — the equation parameter.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier. </p>

## Output

<p>Print -1, if the equation doesn't have integer positive roots. Otherwise print such smallest integer <span class="tex-span"><i>x</i></span> <span class="tex-span">(<i>x</i> &gt; 0)</span>, that the equation given in the statement holds.</p>





```input1
2

```




```input2
110

```




```input3
4

```




```output1
1

```




```output2
10

```




```output3
-1

```



## Note

<p>In the first test case <span class="tex-span"><i>x</i> = 1</span> is the minimum root. As <span class="tex-span"><i>s</i>(1) = 1</span> and <span class="tex-span">1<sup class="upper-index">2</sup> + 1·1 - 2 = 0</span>.</p><p>In the second test case <span class="tex-span"><i>x</i> = 10</span> is the minimum root. As <span class="tex-span"><i>s</i>(10) = 1 + 0 = 1</span> and <span class="tex-span">10<sup class="upper-index">2</sup> + 1·10 - 110 = 0</span>.</p><p>In the third test case the equation has no roots.</p>
