## Description

<div><p>It is known that fleas in Berland can jump only vertically and horizontally, and the length of the jump is always equal to <span class="tex-span"><i>s</i></span> centimeters. A flea has found herself at the center of some cell of the checked board of the size <span class="tex-span"><i>n</i> × <i>m</i></span> centimeters (each cell is <span class="tex-span">1 × 1</span> centimeters). She can jump as she wishes for an arbitrary number of times, she can even visit a cell more than once. The only restriction is that she cannot jump out of the board.</p><p>The flea can count the amount of cells that she can reach from the starting position <span class="tex-span">(<i>x</i>, <i>y</i>)</span>. Let's denote this amount by <span class="tex-span"><i>d</i><sub class="lower-index"><i>x</i>, <i>y</i></sub></span>. Your task is to find the number of such starting positions <span class="tex-span">(<i>x</i>, <i>y</i>)</span>, which have the maximum possible value of <span class="tex-span"><i>d</i><sub class="lower-index"><i>x</i>, <i>y</i></sub></span>.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>s</i> ≤ 10<sup class="upper-index">6</sup></span>) — length of the board, width of the board and length of the flea's jump.</p></div><div class="output-specification"><p>Output the only integer — the number of the required starting positions of the flea.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>s</i> ≤ 10<sup class="upper-index">6</sup></span>) — length of the board, width of the board and length of the flea's jump.</p>

## Output

<p>Output the only integer — the number of the required starting positions of the flea.</p>





```input1
2 3 1000000

```




```input2
3 3 2

```




```output1
6

```




```output2
4

```


