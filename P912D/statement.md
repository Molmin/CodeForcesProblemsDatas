## Description

<div><p>While Grisha was celebrating New Year with Ded Moroz, Misha gifted Sasha a small rectangular pond of size <span class="tex-span"><i>n</i> × <i>m</i></span>, divided into cells of size <span class="tex-span">1 × 1</span>, inhabited by tiny evil fishes (no more than one fish per cell, otherwise they'll strife!).</p><p>The gift bundle also includes a square scoop of size <span class="tex-span"><i>r</i> × <i>r</i></span>, designed for fishing. If the lower-left corner of the scoop-net is located at cell <span class="tex-span">(<i>x</i>, <i>y</i>)</span>, all fishes inside the square <span class="tex-span">(<i>x</i>, <i>y</i>)...(<i>x</i> + <i>r</i> - 1, <i>y</i> + <i>r</i> - 1)</span> get caught. Note that the scoop-net should lie completely inside the pond when used.</p><p>Unfortunately, Sasha is not that skilled in fishing and hence throws the scoop randomly. In order to not frustrate Sasha, Misha decided to release <span class="tex-span"><i>k</i></span> fishes into the empty pond in such a way that the expected value of the number of caught fishes is as high as possible. Help Misha! In other words, put <span class="tex-span"><i>k</i></span> fishes in the pond into distinct cells in such a way that when the scoop-net is placed into a random position among <span class="tex-span">(<i>n</i> - <i>r</i> + 1)·(<i>m</i> - <i>r</i> + 1)</span> possible positions, the average number of caught fishes is as high as possible.</p></div><div class="input-specification"><p>The only line contains four integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>r</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>r</i> ≤ <i>min</i>(<i>n</i>, <i>m</i>)</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>min</i>(<i>n</i>·<i>m</i>, 10<sup class="upper-index">5</sup>)</span>).</p></div><div class="output-specification"><p>Print a single number&nbsp;— the maximum possible expected number of caught fishes.</p><p>You answer is considered correct, is its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>. Namely, let your answer be <span class="tex-span"><i>a</i></span>, and the jury's answer be <span class="tex-span"><i>b</i></span>. Your answer is considered correct, if <img align="middle" class="tex-formula" src="file://qXOF0yH9.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The only line contains four integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>r</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>r</i> ≤ <i>min</i>(<i>n</i>, <i>m</i>)</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>min</i>(<i>n</i>·<i>m</i>, 10<sup class="upper-index">5</sup>)</span>).</p>

## Output

<p>Print a single number&nbsp;— the maximum possible expected number of caught fishes.</p><p>You answer is considered correct, is its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>. Namely, let your answer be <span class="tex-span"><i>a</i></span>, and the jury's answer be <span class="tex-span"><i>b</i></span>. Your answer is considered correct, if <img align="middle" class="tex-formula" src="file://qXOF0yH9.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
3 3 2 3

```




```input2
12 17 9 40

```




```output1
2.0000000000

```




```output2
32.8333333333

```



## Note

<p>In the first example you can put the fishes in cells <span class="tex-span">(2, 1)</span>, <span class="tex-span">(2, 2)</span>, <span class="tex-span">(2, 3)</span>. In this case, for any of four possible positions of the scoop-net (highlighted with light green), the number of fishes inside is equal to two, and so is the expected value.</p><center> <img class="tex-graphics" height="125px" src="file://AU0n3RhJ.png" style="max-width: 100.0%;max-height: 100.0%;" width="567px"> </center>
