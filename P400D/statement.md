## Description

<div><p>Dima took up the biology of bacteria, as a result of his experiments, he invented <span class="tex-span"><i>k</i></span> types of bacteria. Overall, there are <span class="tex-span"><i>n</i></span> bacteria at his laboratory right now, and the number of bacteria of type <span class="tex-span"><i>i</i></span> equals <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>. For convenience, we will assume that all the bacteria are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The bacteria of type <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> are numbered from <img align="middle" class="tex-formula" src="file://Wo5Yrmwo.png" style="max-width: 100.0%;max-height: 100.0%;"> to <img align="middle" class="tex-formula" src="file://71HH8Lfy.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>With the help of special equipment Dima can move energy from some bacteria into some other one. Of course, the use of such equipment is not free. Dima knows <span class="tex-span"><i>m</i></span> ways to move energy from some bacteria to another one. The way with number <span class="tex-span"><i>i</i></span> can be described with integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> mean that this way allows moving energy from bacteria with number <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> to bacteria with number <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> or vice versa for <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> dollars.</p><p>Dima's Chef (Inna) calls the type-distribution <span class="tex-font-style-it">correct</span> if there is a way (may be non-direct) to move energy from any bacteria of the particular type to any other bacteria of the same type (between any two bacteria of the same type) for zero cost.</p><p>As for correct type-distribution the cost of moving the energy depends only on the types of bacteria help Inna to determine is the type-distribution correct? If it is, print the matrix <span class="tex-span"><i>d</i></span> with size <span class="tex-span"><i>k</i> × <i>k</i></span>. Cell <span class="tex-span"><i>d</i>[<i>i</i>][<i>j</i>]</span> of this matrix must be equal to the minimal possible cost of energy-moving from bacteria with type <span class="tex-span"><i>i</i></span> to bacteria with type <span class="tex-span"><i>j</i></span>.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>k</i> ≤ 500)</span>. The next line contains <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>k</i></sub></span> <span class="tex-span">(1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>. Each of the next <span class="tex-span"><i>m</i></span> lines contains three integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>;&nbsp;0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup>)</span>. It is guaranteed that <img align="middle" class="tex-formula" src="file://vLmXH7vt.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div><div class="output-specification"><p>If Dima's type-distribution is correct, print string «<span class="tex-font-style-tt">Yes</span>», and then <span class="tex-span"><i>k</i></span> lines: in the <span class="tex-span"><i>i</i></span>-th line print integers <span class="tex-span"><i>d</i>[<i>i</i>][1], <i>d</i>[<i>i</i>][2], ..., <i>d</i>[<i>i</i>][<i>k</i>]</span> <span class="tex-span">(<i>d</i>[<i>i</i>][<i>i</i>] = 0)</span>. If there is no way to move energy from bacteria <span class="tex-span"><i>i</i></span> to bacteria <span class="tex-span"><i>j</i></span> appropriate <span class="tex-span"><i>d</i>[<i>i</i>][<i>j</i>]</span> must equal to -1. If the type-distribution isn't correct print «<span class="tex-font-style-tt">No</span>».</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>k</i> ≤ 500)</span>. The next line contains <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>k</i></sub></span> <span class="tex-span">(1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>. Each of the next <span class="tex-span"><i>m</i></span> lines contains three integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>;&nbsp;0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup>)</span>. It is guaranteed that <img align="middle" class="tex-formula" src="file://vLmXH7vt.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>

## Output

<p>If Dima's type-distribution is correct, print string «<span class="tex-font-style-tt">Yes</span>», and then <span class="tex-span"><i>k</i></span> lines: in the <span class="tex-span"><i>i</i></span>-th line print integers <span class="tex-span"><i>d</i>[<i>i</i>][1], <i>d</i>[<i>i</i>][2], ..., <i>d</i>[<i>i</i>][<i>k</i>]</span> <span class="tex-span">(<i>d</i>[<i>i</i>][<i>i</i>] = 0)</span>. If there is no way to move energy from bacteria <span class="tex-span"><i>i</i></span> to bacteria <span class="tex-span"><i>j</i></span> appropriate <span class="tex-span"><i>d</i>[<i>i</i>][<i>j</i>]</span> must equal to -1. If the type-distribution isn't correct print «<span class="tex-font-style-tt">No</span>».</p>





```input1
4 4 2
1 3
2 3 0
3 4 0
2 4 1
2 1 2

```




```input2
3 1 2
2 1
1 2 0

```




```input3
3 2 2
2 1
1 2 0
2 3 1

```




```input4
3 0 2
1 2

```




```output1
Yes
0 2
2 0

```




```output2
Yes
0 -1
-1 0

```




```output3
Yes
0 1
1 0

```




```output4
No

```


