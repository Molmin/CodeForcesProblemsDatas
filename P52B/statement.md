## Description

<div><p>You are given a <span class="tex-span"><i>n</i> × <i>m</i></span> field consisting only of periods (<span class="tex-font-style-tt">'.'</span>) and asterisks (<span class="tex-font-style-tt">'*'</span>). Your task is to count all right triangles with two sides parallel to the square sides, whose vertices are in the centers of <span class="tex-font-style-tt">'*'</span>-cells. A right triangle is a triangle in which one angle is a right angle (that is, a 90 degree angle).</p></div><div class="input-specification"><p>The first line contains two positive integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>). The following <span class="tex-span"><i>n</i></span> lines consist of <span class="tex-span"><i>m</i></span> characters each, describing the field. Only <span class="tex-font-style-tt">'.'</span> and <span class="tex-font-style-tt">'*'</span> are allowed.</p></div><div class="output-specification"><p>Output a single number — total number of square triangles in the field. Please, do not use <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preffered to use <span class="tex-font-style-tt">cout</span> (also you may use <span class="tex-font-style-tt">%I64d</span>).</p></div>

## Input

<p>The first line contains two positive integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>). The following <span class="tex-span"><i>n</i></span> lines consist of <span class="tex-span"><i>m</i></span> characters each, describing the field. Only <span class="tex-font-style-tt">'.'</span> and <span class="tex-font-style-tt">'*'</span> are allowed.</p>

## Output

<p>Output a single number — total number of square triangles in the field. Please, do not use <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preffered to use <span class="tex-font-style-tt">cout</span> (also you may use <span class="tex-font-style-tt">%I64d</span>).</p>





```input1
2 2
**
*.

```




```input2
3 4
*..*
.**.
*.**

```




```output1
1

```




```output2
9

```


