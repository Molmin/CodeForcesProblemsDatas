## Description

<div><p>Polycarpus loves hamburgers very much. He especially adores the hamburgers he makes with his own hands. Polycarpus thinks that there are only three decent ingredients to make hamburgers from: a bread, sausage and cheese. He writes down the recipe of his favorite "Le Hamburger de Polycarpus" as a string of letters '<span class="tex-font-style-tt">B</span>' (bread), '<span class="tex-font-style-tt">S</span>' (sausage) и '<span class="tex-font-style-tt">C</span>' (cheese). The ingredients in the recipe go from bottom to top, for example, recipe "<span class="tex-font-style-tt">ВSCBS</span>" represents the hamburger where the ingredients go from bottom to top as bread, sausage, cheese, bread and sausage again.</p><p>Polycarpus has <span class="tex-span"><i>n</i><sub class="lower-index"><i>b</i></sub></span> pieces of bread, <span class="tex-span"><i>n</i><sub class="lower-index"><i>s</i></sub></span> pieces of sausage and <span class="tex-span"><i>n</i><sub class="lower-index"><i>c</i></sub></span> pieces of cheese in the kitchen. Besides, the shop nearby has all three ingredients, the prices are <span class="tex-span"><i>p</i><sub class="lower-index"><i>b</i></sub></span> rubles for a piece of bread, <span class="tex-span"><i>p</i><sub class="lower-index"><i>s</i></sub></span> for a piece of sausage and <span class="tex-span"><i>p</i><sub class="lower-index"><i>c</i></sub></span> for a piece of cheese.</p><p>Polycarpus has <span class="tex-span"><i>r</i></span> rubles and he is ready to shop on them. What maximum number of hamburgers can he cook? You can assume that Polycarpus cannot break or slice any of the pieces of bread, sausage or cheese. Besides, the shop has an unlimited number of pieces of each ingredient.</p></div><div class="input-specification"><p>The first line of the input contains a non-empty string that describes the recipe of "Le Hamburger de Polycarpus". The length of the string doesn't exceed 100, the string contains only letters '<span class="tex-font-style-tt">B</span>' (uppercase English <span class="tex-font-style-tt">B</span>), '<span class="tex-font-style-tt">S</span>' (uppercase English <span class="tex-font-style-tt">S</span>) and '<span class="tex-font-style-tt">C</span>' (uppercase English <span class="tex-font-style-tt">C</span>).</p><p>The second line contains three integers <span class="tex-span"><i>n</i><sub class="lower-index"><i>b</i></sub></span>, <span class="tex-span"><i>n</i><sub class="lower-index"><i>s</i></sub></span>, <span class="tex-span"><i>n</i><sub class="lower-index"><i>c</i></sub></span> (<span class="tex-span">1 ≤ <i>n</i><sub class="lower-index"><i>b</i></sub>, <i>n</i><sub class="lower-index"><i>s</i></sub>, <i>n</i><sub class="lower-index"><i>c</i></sub> ≤ 100</span>) — the number of the pieces of bread, sausage and cheese on Polycarpus' kitchen. The third line contains three integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>b</i></sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>s</i></sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>c</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>b</i></sub>, <i>p</i><sub class="lower-index"><i>s</i></sub>, <i>p</i><sub class="lower-index"><i>c</i></sub> ≤ 100</span>) — the price of one piece of bread, sausage and cheese in the shop. Finally, the fourth line contains integer <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>r</i> ≤ 10<sup class="upper-index">12</sup></span>) — the number of rubles Polycarpus has.</p><p>Please, do not write the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div><div class="output-specification"><p>Print the maximum number of hamburgers Polycarpus can make. If he can't make any hamburger, print <span class="tex-font-style-tt">0</span>.</p></div>

## Input

<p>The first line of the input contains a non-empty string that describes the recipe of "Le Hamburger de Polycarpus". The length of the string doesn't exceed 100, the string contains only letters '<span class="tex-font-style-tt">B</span>' (uppercase English <span class="tex-font-style-tt">B</span>), '<span class="tex-font-style-tt">S</span>' (uppercase English <span class="tex-font-style-tt">S</span>) and '<span class="tex-font-style-tt">C</span>' (uppercase English <span class="tex-font-style-tt">C</span>).</p><p>The second line contains three integers <span class="tex-span"><i>n</i><sub class="lower-index"><i>b</i></sub></span>, <span class="tex-span"><i>n</i><sub class="lower-index"><i>s</i></sub></span>, <span class="tex-span"><i>n</i><sub class="lower-index"><i>c</i></sub></span> (<span class="tex-span">1 ≤ <i>n</i><sub class="lower-index"><i>b</i></sub>, <i>n</i><sub class="lower-index"><i>s</i></sub>, <i>n</i><sub class="lower-index"><i>c</i></sub> ≤ 100</span>) — the number of the pieces of bread, sausage and cheese on Polycarpus' kitchen. The third line contains three integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>b</i></sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>s</i></sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>c</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>b</i></sub>, <i>p</i><sub class="lower-index"><i>s</i></sub>, <i>p</i><sub class="lower-index"><i>c</i></sub> ≤ 100</span>) — the price of one piece of bread, sausage and cheese in the shop. Finally, the fourth line contains integer <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>r</i> ≤ 10<sup class="upper-index">12</sup></span>) — the number of rubles Polycarpus has.</p><p>Please, do not write the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>

## Output

<p>Print the maximum number of hamburgers Polycarpus can make. If he can't make any hamburger, print <span class="tex-font-style-tt">0</span>.</p>





```input1
BBBSSC
6 4 1
1 2 3
4

```




```input2
BBC
1 10 1
1 10 1
21

```




```input3
BSC
1 1 1
1 1 3
1000000000000

```




```output1
2

```




```output2
7

```




```output3
200000000001

```


