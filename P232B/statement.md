## Description

<div><p>John Doe has an <span class="tex-span"><i>n</i> × <i>m</i></span> table. John Doe can paint points in some table cells, not more than one point in one table cell. John Doe wants to use such operations to make each square subtable of size <span class="tex-span"><i>n</i> × <i>n</i></span> have exactly <span class="tex-span"><i>k</i></span> points.</p><p>John Doe wondered, how many distinct ways to fill the table with points are there, provided that the condition must hold. As this number can be rather large, John Doe asks to find its remainder after dividing by <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p><p>You should assume that John always paints a point exactly in the center of some cell. Two ways to fill a table are considered distinct, if there exists a table cell, that has a point in one way and doesn't have it in the other.</p></div><div class="input-specification"><p>A single line contains space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100;&nbsp;<i>n</i> ≤ <i>m</i> ≤ 10<sup class="upper-index">18</sup>;&nbsp;0 ≤ <i>k</i> ≤ <i>n</i><sup class="upper-index">2</sup></span>) — the number of rows of the table, the number of columns of the table and the number of points each square must contain.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier. </p></div><div class="output-specification"><p>In a single line print a single integer — the remainder from dividing the described number of ways by <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>A single line contains space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100;&nbsp;<i>n</i> ≤ <i>m</i> ≤ 10<sup class="upper-index">18</sup>;&nbsp;0 ≤ <i>k</i> ≤ <i>n</i><sup class="upper-index">2</sup></span>) — the number of rows of the table, the number of columns of the table and the number of points each square must contain.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier. </p>

## Output

<p>In a single line print a single integer — the remainder from dividing the described number of ways by <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
5 6 1

```




```output1
45
```



## Note

<p>Let's consider the first test case:  </p><center> <img class="tex-graphics" src="file://s6MH99Jl.png" style="max-width: 100.0%;max-height: 100.0%;">  </center> The gray area belongs to both <span class="tex-span">5 × 5</span> squares. So, if it has one point, then there shouldn't be points in any other place. If one of the white areas has a point, then the other one also must have a point. Thus, there are about <span class="tex-span">20</span> variants, where the point lies in the gray area and <span class="tex-span">25</span> variants, where each of the white areas contains a point. Overall there are <span class="tex-span">45</span> variants.
