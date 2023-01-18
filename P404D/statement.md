## Description

<div><p>Game "Minesweeper 1D" is played on a line of squares, the line's height is 1 square, the line's width is <span class="tex-span"><i>n</i></span> squares. Some of the squares contain bombs. If a square doesn't contain a bomb, then it contains a number from 0 to 2 — the total number of bombs in adjacent squares.</p><p>For example, the correct field to play looks like that: <span class="tex-font-style-tt">001*2***101*</span>. The cells that are marked with "<span class="tex-font-style-tt">*</span>" contain bombs. Note that on the correct field the numbers represent the number of bombs in adjacent cells. For example, field <span class="tex-font-style-tt">2*</span> is not correct, because cell with value 2 must have two adjacent cells with bombs.</p><p>Valera wants to make a correct field to play "Minesweeper 1D". He has already painted a squared field with width of <span class="tex-span"><i>n</i></span> cells, put several bombs on the field and wrote numbers into some cells. Now he wonders how many ways to fill the remaining cells with bombs and numbers are there if we should get a correct field in the end.</p></div><div class="input-specification"><p>The first line contains sequence of characters without spaces <span class="tex-span"><i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>)</span>, containing only characters "<span class="tex-font-style-tt">*</span>", "<span class="tex-font-style-tt">?</span>" and digits "<span class="tex-font-style-tt">0</span>", "<span class="tex-font-style-tt">1</span>" or "<span class="tex-font-style-tt">2</span>". If character <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> equals "<span class="tex-font-style-tt">*</span>", then the <span class="tex-span"><i>i</i></span>-th cell of the field contains a bomb. If character <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> equals "<span class="tex-font-style-tt">?</span>", then Valera hasn't yet decided what to put in the <span class="tex-span"><i>i</i></span>-th cell. Character <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>, that is equal to a digit, represents the digit written in the <span class="tex-span"><i>i</i></span>-th square.</p></div><div class="output-specification"><p>Print a single integer — the number of ways Valera can fill the empty cells and get a correct field.</p><p>As the answer can be rather large, print it modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains sequence of characters without spaces <span class="tex-span"><i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>)</span>, containing only characters "<span class="tex-font-style-tt">*</span>", "<span class="tex-font-style-tt">?</span>" and digits "<span class="tex-font-style-tt">0</span>", "<span class="tex-font-style-tt">1</span>" or "<span class="tex-font-style-tt">2</span>". If character <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> equals "<span class="tex-font-style-tt">*</span>", then the <span class="tex-span"><i>i</i></span>-th cell of the field contains a bomb. If character <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> equals "<span class="tex-font-style-tt">?</span>", then Valera hasn't yet decided what to put in the <span class="tex-span"><i>i</i></span>-th cell. Character <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>, that is equal to a digit, represents the digit written in the <span class="tex-span"><i>i</i></span>-th square.</p>

## Output

<p>Print a single integer — the number of ways Valera can fill the empty cells and get a correct field.</p><p>As the answer can be rather large, print it modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
?01???

```




```input2
?

```




```input3
**12

```




```input4
1

```




```output1
4

```




```output2
2

```




```output3
0

```




```output4
0

```



## Note

<p>In the first test sample you can get the following correct fields: <span class="tex-font-style-tt">001**1</span>, <span class="tex-font-style-tt">001***</span>, <span class="tex-font-style-tt">001*2*</span>, <span class="tex-font-style-tt">001*10</span>.</p>
