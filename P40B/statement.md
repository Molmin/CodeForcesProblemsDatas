## Description

<div><p>A chessboard <span class="tex-span"><i>n</i> × <i>m</i></span> in size is given. During the zero minute we repaint all the black squares to the 0 color. During the <span class="tex-span"><i>i</i></span>-th minute we repaint to the <span class="tex-span"><i>i</i></span> color the <span class="tex-font-style-bf">initially black</span> squares that have exactly four corner-adjacent squares painted <span class="tex-span"><i>i</i> - 1</span> (all such squares are repainted simultaneously). This process continues ad infinitum. You have to figure out how many squares we repainted exactly <span class="tex-span"><i>x</i></span> times.</p><p>The upper left square of the board has to be assumed to be always black. Two squares are called corner-adjacent, if they have exactly one common point.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 5000</span>). The second line contains integer <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print how many squares will be painted exactly <span class="tex-span"><i>x</i></span> times.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 5000</span>). The second line contains integer <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print how many squares will be painted exactly <span class="tex-span"><i>x</i></span> times.</p>





```input1
3 3
1

```




```input2
3 3
2

```




```input3
1 1
1

```




```output1
4

```




```output2
1

```




```output3
1

```


