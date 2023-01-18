## Description

<div><p>Little Janet likes playing with cubes. Actually, she likes to play with anything whatsoever, cubes or tesseracts, as long as they are multicolored. Each cube is described by two parameters — color <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and size <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>. A Zebra Tower is a tower that consists of cubes of exactly two colors. Besides, the colors of the cubes in the tower must alternate (colors of adjacent cubes must differ). The Zebra Tower should have at least two cubes. There are no other limitations. The figure below shows an example of a Zebra Tower.</p><center> <img class="tex-graphics" src="file://FZdaLuym.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>A Zebra Tower's height is the sum of sizes of all cubes that form the tower. Help little Janet build the Zebra Tower of the maximum possible height, using the available cubes.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of cubes. Next <span class="tex-span"><i>n</i></span> lines contain the descriptions of the cubes, one description per line. A cube description consists of two space-separated integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the <span class="tex-span"><i>i</i></span>-th cube's color and size, correspondingly. It is guaranteed that there are at least two cubes of different colors.</p></div><div class="output-specification"><p>Print the description of the Zebra Tower of the maximum height in the following form. In the first line print the tower's height, in the second line print the number of cubes that form the tower, and in the third line print the space-separated indices of cubes in the order in which they follow in the tower from the bottom to the top. Assume that the cubes are numbered from 1 to <span class="tex-span"><i>n</i></span> in the order in which they were given in the input.</p><p>If there are several existing Zebra Towers with maximum heights, it is allowed to print any of them. </p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specificator.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of cubes. Next <span class="tex-span"><i>n</i></span> lines contain the descriptions of the cubes, one description per line. A cube description consists of two space-separated integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the <span class="tex-span"><i>i</i></span>-th cube's color and size, correspondingly. It is guaranteed that there are at least two cubes of different colors.</p>

## Output

<p>Print the description of the Zebra Tower of the maximum height in the following form. In the first line print the tower's height, in the second line print the number of cubes that form the tower, and in the third line print the space-separated indices of cubes in the order in which they follow in the tower from the bottom to the top. Assume that the cubes are numbered from 1 to <span class="tex-span"><i>n</i></span> in the order in which they were given in the input.</p><p>If there are several existing Zebra Towers with maximum heights, it is allowed to print any of them. </p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specificator.</p>





```input1
4
1 2
1 3
2 4
3 3

```




```input2
2
1 1
2 1

```




```output1
9
3
2 3 1 

```




```output2
2
2
2 1 

```


