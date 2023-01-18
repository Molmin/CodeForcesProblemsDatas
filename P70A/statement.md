## Description

<div><p>Fangy collects cookies. Once he decided to take a box and put cookies into it in some way. If we take a square <span class="tex-span"><i>k</i> × <i>k</i></span> in size, divided into blocks <span class="tex-span">1 × 1</span> in size and paint there the main diagonal together with cells, which lie above it, then the painted area will be equal to the area occupied by one cookie <span class="tex-span"><i>k</i></span> in size. Fangy also has a box with a square base <span class="tex-span">2<sup class="upper-index"><i>n</i></sup> × 2<sup class="upper-index"><i>n</i></sup></span>, divided into blocks <span class="tex-span">1 × 1</span> in size. In a box the cookies should not overlap, and they should not be turned over or rotated. See cookies of sizes <span class="tex-span">2</span> and <span class="tex-span">4</span> respectively on the figure: </p><center> <img class="tex-graphics" src="file://chVvAPwC.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> <p>To stack the cookies the little walrus uses the following algorithm. He takes out of the repository the largest cookie which can fit in some place in the box and puts it there. Everything could be perfect but alas, in the repository the little walrus has infinitely many cookies of size <span class="tex-span">2</span> and larger, and there are no cookies of size <span class="tex-span">1</span>, therefore, empty cells will remain in the box. Fangy wants to know how many empty cells will be left in the end.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 1000</span>).</p></div><div class="output-specification"><p>Print the single number, equal to the number of empty cells in the box. The answer should be printed modulo <span class="tex-span">10<sup class="upper-index">6</sup> + 3</span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 1000</span>).</p>

## Output

<p>Print the single number, equal to the number of empty cells in the box. The answer should be printed modulo <span class="tex-span">10<sup class="upper-index">6</sup> + 3</span>.</p>





```input1
3

```




```output1
9
```



## Note

<p>If the box possesses the base of <span class="tex-span">2<sup class="upper-index">3</sup> × 2<sup class="upper-index">3</sup></span> (as in the example), then the cookies will be put there in the following manner: </p><center><img class="tex-graphics" src="file://9AdJBCVV.png" style="max-width: 100.0%;max-height: 100.0%;"></center>
