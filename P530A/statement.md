## Description

<div><p>You are given a quadratic equation with integer coefficients <span class="tex-span"><i>A</i> * <i>X</i><sup class="upper-index">2</sup> + <i>B</i> * <i>X</i> + <i>C</i> = 0</span>. It is guaranteed that <span class="tex-span"><i>A</i> ≠ 0</span> and that the equation has at least one real root. Output the roots of the equation.</p></div><div class="input-specification"><p>The only line of input contains integers <span class="tex-span"><i>A</i>, <i>B</i></span> and <span class="tex-span"><i>C</i></span> (<span class="tex-span"> - 1000 ≤ <i>A</i>, <i>B</i>, <i>C</i> ≤ 1000, <i>A</i> ≠ 0</span>), separated by spaces.</p></div><div class="output-specification"><p>Output the roots of the equation in increasing order. If the equation has a single root of multiplicity 2, output it once. The root is considered to be correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p></div>

## Input

<p>The only line of input contains integers <span class="tex-span"><i>A</i>, <i>B</i></span> and <span class="tex-span"><i>C</i></span> (<span class="tex-span"> - 1000 ≤ <i>A</i>, <i>B</i>, <i>C</i> ≤ 1000, <i>A</i> ≠ 0</span>), separated by spaces.</p>

## Output

<p>Output the roots of the equation in increasing order. If the equation has a single root of multiplicity 2, output it once. The root is considered to be correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p>





```input1
1 -2 1

```




```input2
1 0 -1

```




```input3
2 -3 1

```




```output1
1

```




```output2
-1 1

```




```output3
0.5 1

```


