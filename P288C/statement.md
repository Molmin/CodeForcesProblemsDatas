## Description

<div><p>Little penguin Polo likes permutations. But most of all he likes permutations of integers from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i></span>, inclusive.</p><p>For permutation <span class="tex-span"><i>p</i> = <i>p</i><sub class="lower-index">0</sub>, <i>p</i><sub class="lower-index">1</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span>, Polo has defined its beauty — number <img align="middle" class="tex-formula" src="file://mv3tsmGj.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Expression <img align="middle" class="tex-formula" src="file://5IX3ILD6.png" style="max-width: 100.0%;max-height: 100.0%;"> means applying the operation of bitwise excluding "OR" to numbers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>. This operation exists in all modern programming languages, for example, in language <span class="tex-font-style-it">C++</span> and <span class="tex-font-style-it">Java</span> it is represented as "<span class="tex-font-style-tt">^</span>" and in <span class="tex-font-style-it">Pascal</span> — as "<span class="tex-font-style-tt">xor</span>".</p><p>Help him find among all permutations of integers from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i></span> the permutation with the maximum beauty.</p></div><div class="input-specification"><p>The single line contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>).</p></div><div class="output-specification"><p>In the first line print integer <span class="tex-span"><i>m</i></span> the maximum possible beauty. In the second line print any permutation of integers from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i></span> with the beauty equal to <span class="tex-span"><i>m</i></span>.</p><p>If there are several suitable permutations, you are allowed to print any of them.</p></div>

## Input

<p>The single line contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>).</p>

## Output

<p>In the first line print integer <span class="tex-span"><i>m</i></span> the maximum possible beauty. In the second line print any permutation of integers from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i></span> with the beauty equal to <span class="tex-span"><i>m</i></span>.</p><p>If there are several suitable permutations, you are allowed to print any of them.</p>





```input1
4

```




```output1
20
0 2 1 4 3

```


