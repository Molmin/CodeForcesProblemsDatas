## Description

<div><p>A long time ago in some far country lived king Copa. After the recent king's reform, he got so large powers that started to keep the books by himself.</p><p>The total income <span class="tex-span"><i>A</i></span> of his kingdom during <span class="tex-span">0</span>-th year is known, as well as the total income <span class="tex-span"><i>B</i></span> during <span class="tex-span"><i>n</i></span>-th year (these numbers can be negative — it means that there was a loss in the correspondent year). </p><p>King wants to show financial stability. To do this, he needs to find common coefficient <span class="tex-span"><i>X</i></span> — the coefficient of income growth during one year. This coefficient should satisfy the equation:</p><center class="tex-equation"><span class="tex-span"><i>A</i>·<i>X</i><sup class="upper-index"><i>n</i></sup> = <i>B</i>.</span></center><p>Surely, the king is not going to do this job by himself, and demands you to find such number <span class="tex-span"><i>X</i></span>.</p><p>It is necessary to point out that the fractional numbers are not used in kingdom's economy. That's why all input numbers as well as coefficient <span class="tex-span"><i>X</i></span> must be integers. The number <span class="tex-span"><i>X</i></span> may be zero or negative.</p></div><div class="input-specification"><p>The input contains three integers <span class="tex-span"><i>A</i></span>, <span class="tex-span"><i>B</i></span>, <span class="tex-span"><i>n</i></span> (<span class="tex-span">|<i>A</i>|, |<i>B</i>| ≤ 1000</span>, <span class="tex-span">1 ≤ <i>n</i> ≤ 10</span>).</p></div><div class="output-specification"><p>Output the required integer coefficient <span class="tex-span"><i>X</i></span>, or «No solution», if such a coefficient does not exist or it is fractional. If there are several possible solutions, output any of them.</p></div>

## Input

<p>The input contains three integers <span class="tex-span"><i>A</i></span>, <span class="tex-span"><i>B</i></span>, <span class="tex-span"><i>n</i></span> (<span class="tex-span">|<i>A</i>|, |<i>B</i>| ≤ 1000</span>, <span class="tex-span">1 ≤ <i>n</i> ≤ 10</span>).</p>

## Output

<p>Output the required integer coefficient <span class="tex-span"><i>X</i></span>, or «No solution», if such a coefficient does not exist or it is fractional. If there are several possible solutions, output any of them.</p>





```input1
2 18 2

```




```input2
-1 8 3

```




```input3
0 0 10

```




```input4
1 16 5

```




```output1
3
```




```output2
-2
```




```output3
5
```




```output4
No solution
```


