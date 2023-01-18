## Description

<div><p>Let's imagine: there is a chess piece <span class="tex-font-style-it">billiard ball</span>. Its movements resemble the ones of a bishop chess piece. The only difference is that when a billiard ball hits the board's border, it can reflect from it and continue moving.</p><p>More formally, first one of four diagonal directions is chosen and the billiard ball moves in that direction. When it reaches the square located on the board's edge, the billiard ball reflects from it; it changes the direction of its movement by 90 degrees and continues moving. Specifically, having reached a corner square, the billiard ball is reflected twice and starts to move the opposite way. While it moves, the billiard ball can make an infinite number of reflections. At any square of its trajectory the billiard ball can stop and on that the move is considered completed.</p><center> <img class="tex-graphics" src="file://PaCyE9A5.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>It is considered that one billiard ball <span class="tex-span"><i>a</i></span> beats another billiard ball <span class="tex-span"><i>b</i></span> if <span class="tex-span"><i>a</i></span> can reach a point where <span class="tex-span"><i>b</i></span> is located.</p><p>You are suggested to find the maximal number of billiard balls, that pairwise do not beat each other and that can be positioned on a chessboard <span class="tex-span"><i>n</i> × <i>m</i></span> in size.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>).</p></div><div class="output-specification"><p>Print a single number, the maximum possible number of billiard balls that do not pairwise beat each other.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit numbers in C++. It is preferred to use <span class="tex-font-style-tt">cin</span> (also you may use the <span class="tex-font-style-tt">%I64d</span> specificator).</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>).</p>

## Output

<p>Print a single number, the maximum possible number of billiard balls that do not pairwise beat each other.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit numbers in C++. It is preferred to use <span class="tex-font-style-tt">cin</span> (also you may use the <span class="tex-font-style-tt">%I64d</span> specificator).</p>





```input1
3 4

```




```input2
3 3

```




```output1
2
```




```output2
3
```


