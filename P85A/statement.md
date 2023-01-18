## Description

<div><p>We all know the problem about the number of ways one can tile a <span class="tex-span">2 × <i>n</i></span> field by <span class="tex-span">1 × 2</span> dominoes. You probably remember that it goes down to Fibonacci numbers. We will talk about some other problem below, there you also are going to deal with tiling a rectangular field with dominoes.</p><p>You are given a <span class="tex-span">4 × <i>n</i></span> rectangular field, that is the field that contains four lines and <span class="tex-span"><i>n</i></span> columns. You have to find for it any tiling by <span class="tex-span">1 × 2</span> dominoes such that each of the <span class="tex-span"><i>n</i> - 1</span> potential vertical cuts along the grid lines intersects at least one domino, splitting it in two. No two dominoes in the sought tiling should overlap, each square of the field should be covered by exactly one domino. It is allowed to rotate the dominoes, that is, you can use <span class="tex-span">2 × 1</span> as well as <span class="tex-span">1 × 2</span> dominoes.</p><p>Write a program that finds an arbitrary sought tiling. </p></div><div class="input-specification"><p>The input contains one positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of the field's columns.</p></div><div class="output-specification"><p>If there's no solution, print "-1" (without the quotes). Otherwise, print four lines containing <span class="tex-span"><i>n</i></span> characters each — that's the description of tiling, where each vertical cut intersects at least one domino. You should print the tiling, having painted the field in no more than <span class="tex-span">26</span> colors. Each domino should be painted a color. Different dominoes can be painted the same color, but dominoes of the same color should not be side-neighbouring. To indicate colors you should use lowercase Latin letters. Print any of the acceptable ways of tiling.</p></div>

## Input

<p>The input contains one positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of the field's columns.</p>

## Output

<p>If there's no solution, print "-1" (without the quotes). Otherwise, print four lines containing <span class="tex-span"><i>n</i></span> characters each — that's the description of tiling, where each vertical cut intersects at least one domino. You should print the tiling, having painted the field in no more than <span class="tex-span">26</span> colors. Each domino should be painted a color. Different dominoes can be painted the same color, but dominoes of the same color should not be side-neighbouring. To indicate colors you should use lowercase Latin letters. Print any of the acceptable ways of tiling.</p>





```input1
4

```




```output1
yyzz
bccd
bxxd
yyaa

```


