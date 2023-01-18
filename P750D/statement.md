## Description

<div><p>One tradition of welcoming the New Year is launching fireworks into the sky. Usually a launched firework flies vertically upward for some period of time, then explodes, splitting into several parts flying in different directions. Sometimes those parts also explode after some period of time, splitting into even more parts, and so on.</p><p>Limak, who lives in an infinite grid, has a single firework. The behaviour of the firework is described with a recursion depth <span class="tex-span"><i>n</i></span> and a duration for each level of recursion <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span>. Once Limak launches the firework in some cell, the firework starts moving upward. After covering <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span> cells (including the starting cell), it explodes and splits into two parts, each moving in the direction changed by <span class="tex-span">45</span> degrees (see the pictures below for clarification). So, one part moves in the top-left direction, while the other one moves in the top-right direction. Each part explodes again after covering <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span> cells, splitting into two parts moving in directions again changed by <span class="tex-span">45</span> degrees. The process continues till the <span class="tex-span"><i>n</i></span>-th level of recursion, when all <span class="tex-span">2<sup class="upper-index"><i>n</i> - 1</sup></span> existing parts explode and disappear without creating new parts. After a few levels of recursion, it's possible that some parts will be at the same place and at the same time&nbsp;— it is allowed and such parts do not crash.</p><p>Before launching the firework, Limak must make sure that nobody stands in cells which will be visited at least once by the firework. Can you count the number of those cells?</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 30</span>)&nbsp;— the total depth of the recursion.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 5</span>). On the <span class="tex-span"><i>i</i></span>-th level each of <span class="tex-span">2<sup class="upper-index"><i>i</i> - 1</sup></span> parts will cover <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> cells before exploding.</p></div><div class="output-specification"><p>Print one integer, denoting the number of cells which will be visited at least once by any part of the firework.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 30</span>)&nbsp;— the total depth of the recursion.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 5</span>). On the <span class="tex-span"><i>i</i></span>-th level each of <span class="tex-span">2<sup class="upper-index"><i>i</i> - 1</sup></span> parts will cover <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> cells before exploding.</p>

## Output

<p>Print one integer, denoting the number of cells which will be visited at least once by any part of the firework.</p>





```input1
4
4 2 2 3

```




```input2
6
1 1 1 1 1 3

```




```input3
1
3

```




```output1
39

```




```output2
85

```




```output3
3

```



## Note

<p>For the first sample, the drawings below show the situation after each level of recursion. Limak launched the firework from the bottom-most red cell. It covered <span class="tex-span"><i>t</i><sub class="lower-index">1</sub> = 4</span> cells (marked red), exploded and divided into two parts (their further movement is marked green). All explosions are marked with an '<span class="tex-font-style-tt">X</span>' character. On the last drawing, there are <span class="tex-span">4</span> red, <span class="tex-span">4</span> green, <span class="tex-span">8</span> orange and <span class="tex-span">23</span> pink cells. So, the total number of visited cells is <span class="tex-span">4 + 4 + 8 + 23 = 39</span>.</p><center> <img class="tex-graphics" src="file://opNuPqSQ.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>For the second sample, the drawings below show the situation after levels <span class="tex-span">4</span>, <span class="tex-span">5</span> and <span class="tex-span">6</span>. The middle drawing shows directions of all parts that will move in the next level.</p><center> <img class="tex-graphics" src="file://y9YCZf59.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
