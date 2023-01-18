## Description

<div><p>Three companies decided to order a billboard with pictures of their logos. A billboard is a big <span class="tex-font-style-it">square</span> board. A logo of each company is a rectangle of a non-zero area. </p><p>Advertisers will put up the ad only if it is possible to place all three logos on the billboard so that they do not overlap and the billboard has no empty space left. When you put a logo on the billboard, you should rotate it so that the sides were parallel to the sides of the billboard.</p><p>Your task is to determine if it is possible to put the logos of all the three companies on some square billboard without breaking any of the described rules.</p></div><div class="input-specification"><p>The first line of the input contains six positive integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>, <i>x</i><sub class="lower-index">3</sub>, <i>y</i><sub class="lower-index">3</sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>, <i>x</i><sub class="lower-index">3</sub>, <i>y</i><sub class="lower-index">3</sub> ≤ 100</span>), where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> determine the length and width of the logo of the <span class="tex-span"><i>i</i></span>-th company respectively.</p></div><div class="output-specification"><p>If it is impossible to place all the three logos on a square shield, print a single integer "<span class="tex-font-style-tt">-1</span>" (without the quotes).</p><p>If it is possible, print in the first line the length of a side of square <span class="tex-span"><i>n</i></span>, where you can place all the three logos. Each of the next <span class="tex-span"><i>n</i></span> lines should contain <span class="tex-span"><i>n</i></span> uppercase English letters "<span class="tex-font-style-tt">A</span>", "<span class="tex-font-style-tt">B</span>" or "<span class="tex-font-style-tt">C</span>". The sets of the same letters should form solid rectangles, provided that:</p><ul> <li> the sizes of the rectangle composed from letters "<span class="tex-font-style-tt">A</span>" should be equal to the sizes of the logo of the first company, </li><li> the sizes of the rectangle composed from letters "<span class="tex-font-style-tt">B</span>" should be equal to the sizes of the logo of the second company, </li><li> the sizes of the rectangle composed from letters "<span class="tex-font-style-tt">C</span>" should be equal to the sizes of the logo of the third company, </li></ul><p>Note that the logos of the companies can be rotated for printing on the billboard. The billboard mustn't have any empty space. If a square billboard can be filled with the logos in multiple ways, you are allowed to print any of them.</p><p>See the samples to better understand the statement.</p></div>

## Input

<p>The first line of the input contains six positive integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>, <i>x</i><sub class="lower-index">3</sub>, <i>y</i><sub class="lower-index">3</sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>, <i>x</i><sub class="lower-index">3</sub>, <i>y</i><sub class="lower-index">3</sub> ≤ 100</span>), where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> determine the length and width of the logo of the <span class="tex-span"><i>i</i></span>-th company respectively.</p>

## Output

<p>If it is impossible to place all the three logos on a square shield, print a single integer "<span class="tex-font-style-tt">-1</span>" (without the quotes).</p><p>If it is possible, print in the first line the length of a side of square <span class="tex-span"><i>n</i></span>, where you can place all the three logos. Each of the next <span class="tex-span"><i>n</i></span> lines should contain <span class="tex-span"><i>n</i></span> uppercase English letters "<span class="tex-font-style-tt">A</span>", "<span class="tex-font-style-tt">B</span>" or "<span class="tex-font-style-tt">C</span>". The sets of the same letters should form solid rectangles, provided that:</p><ul> <li> the sizes of the rectangle composed from letters "<span class="tex-font-style-tt">A</span>" should be equal to the sizes of the logo of the first company, </li><li> the sizes of the rectangle composed from letters "<span class="tex-font-style-tt">B</span>" should be equal to the sizes of the logo of the second company, </li><li> the sizes of the rectangle composed from letters "<span class="tex-font-style-tt">C</span>" should be equal to the sizes of the logo of the third company, </li></ul><p>Note that the logos of the companies can be rotated for printing on the billboard. The billboard mustn't have any empty space. If a square billboard can be filled with the logos in multiple ways, you are allowed to print any of them.</p><p>See the samples to better understand the statement.</p>





```input1
5 1 2 5 5 2

```




```input2
4 4 2 6 4 2

```




```output1
5
AAAAA
BBBBB
BBBBB
CCCCC
CCCCC

```




```output2
6
BBBBBB
BBBBBB
AAAACC
AAAACC
AAAACC
AAAACC

```


