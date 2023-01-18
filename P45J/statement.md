## Description

<div><p>Vasya is a <span class="tex-font-style-underline">Greencode</span> wildlife preservation society proponent. One day he found an empty field nobody owned, divided it into <span class="tex-span"><i>n</i> × <i>m</i></span> squares and decided to plant a forest there. Vasya will plant <span class="tex-span"><i>nm</i></span> trees of all different heights from <span class="tex-span">1</span> to <span class="tex-span"><i>nm</i></span>. For his forest to look more natural he wants any two trees growing in the side neighbouring squares to have the absolute value of difference in heights to be strictly more than 1. Help Vasya: make the plan of the forest planting for which this condition is fulfilled.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>) — the number of rows and columns on Vasya's field</p></div><div class="output-specification"><p>If there's no solution, print <span class="tex-font-style-tt">-1</span>. Otherwise, print <span class="tex-span"><i>n</i></span> lines containing <span class="tex-span"><i>m</i></span> numbers each — the trees' planting plan. In every square of the plan the height of a tree that should be planted on this square should be written. If there are several solutions to that problem, print any of them.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>) — the number of rows and columns on Vasya's field</p>

## Output

<p>If there's no solution, print <span class="tex-font-style-tt">-1</span>. Otherwise, print <span class="tex-span"><i>n</i></span> lines containing <span class="tex-span"><i>m</i></span> numbers each — the trees' planting plan. In every square of the plan the height of a tree that should be planted on this square should be written. If there are several solutions to that problem, print any of them.</p>





```input1
2 3

```




```input2
2 1

```




```output1
3 6 2
5 1 4

```




```output2
-1

```


