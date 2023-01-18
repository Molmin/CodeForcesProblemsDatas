## Description

<div><p>There are <span class="tex-span"><i>n</i></span> castles in the Lannister's Kingdom and some walls connect two castles, no two castles are connected by more than one wall, no wall connects a castle to itself. </p><p>Sir Jaime Lannister has discovered that Daenerys Targaryen is going to attack his kingdom soon. Therefore he wants to defend his kingdom. He has <span class="tex-span"><i>k</i></span> liters of a strange liquid. He wants to distribute that liquid among the castles, so each castle may contain some liquid (possibly zero or non-integer number of liters). After that the stability of a wall is defined as follows: if the wall connects two castles <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, and they contain <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> liters of that liquid, respectively, then the strength of that wall is <span class="tex-span"><i>x</i>·<i>y</i></span>.</p><p>Your task is to print the maximum possible sum of stabilities of the walls that Sir Jaime Lannister can achieve.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 40</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 1000</span>).</p><p>Then <span class="tex-span"><i>n</i></span> lines follows. The <span class="tex-span"><i>i</i></span>-th of these lines contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>a</i><sub class="lower-index"><i>i</i>, 2</sub>, ..., <i>a</i><sub class="lower-index"><i>i</i>, <i>n</i></sub></span> (<img align="middle" class="tex-formula" src="file://wabLbtVp.png" style="max-width: 100.0%;max-height: 100.0%;">). If castles <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> are connected by a wall, then <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = 1</span>. Otherwise it is equal to <span class="tex-span">0</span>.</p><p>It is guaranteed that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = <i>a</i><sub class="lower-index"><i>j</i>, <i>i</i></sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>i</i></sub> = 0</span> for all <span class="tex-span">1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i></span>.</p></div><div class="output-specification"><p>Print the maximum possible sum of stabilities of the walls that Sir Jaime Lannister can achieve.</p><p>Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://Nlne1XoS.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 40</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 1000</span>).</p><p>Then <span class="tex-span"><i>n</i></span> lines follows. The <span class="tex-span"><i>i</i></span>-th of these lines contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>a</i><sub class="lower-index"><i>i</i>, 2</sub>, ..., <i>a</i><sub class="lower-index"><i>i</i>, <i>n</i></sub></span> (<img align="middle" class="tex-formula" src="file://wabLbtVp.png" style="max-width: 100.0%;max-height: 100.0%;">). If castles <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> are connected by a wall, then <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = 1</span>. Otherwise it is equal to <span class="tex-span">0</span>.</p><p>It is guaranteed that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = <i>a</i><sub class="lower-index"><i>j</i>, <i>i</i></sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>i</i></sub> = 0</span> for all <span class="tex-span">1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i></span>.</p>

## Output

<p>Print the maximum possible sum of stabilities of the walls that Sir Jaime Lannister can achieve.</p><p>Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://Nlne1XoS.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
3 1
0 1 0
1 0 0
0 0 0

```




```input2
4 4
0 1 0 1
1 0 1 0
0 1 0 1
1 0 1 0

```




```output1
0.250000000000

```




```output2
4.000000000000

```



## Note

<p>In the first sample, we can assign <span class="tex-span">0.5, 0.5, 0</span> liters of liquid to castles <span class="tex-span">1, 2, 3</span>, respectively, to get the maximum sum (<span class="tex-span">0.25</span>).</p><p>In the second sample, we can assign <span class="tex-span">1.0, 1.0, 1.0, 1.0</span> liters of liquid to castles <span class="tex-span">1, 2, 3, 4</span>, respectively, to get the maximum sum (<span class="tex-span">4.0</span>)</p>
