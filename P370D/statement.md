## Description

<div><p>Innocentius has a problem — his computer monitor has broken. Now some of the pixels are "dead", that is, they are always black. As consequence, Innocentius can't play the usual computer games. He is recently playing the following game with his younger brother Polycarpus.</p><p>Innocentius is touch-typing a program that paints a white square one-pixel wide frame on the black screen. As the monitor is broken, some pixels that should be white remain black. Polycarpus should look at what the program displayed on the screen and guess the position and size of the frame Innocentius has painted. Polycarpus doesn't like the game but Innocentius persuaded brother to play as "the game is good for the imagination and attention".</p><p>Help Polycarpus, automatize his part in the gaming process. Write the code that finds such possible <span class="tex-font-style-it">square</span> frame that:</p><ul> <li> the frame's width is 1 pixel, </li><li> the frame doesn't go beyond the borders of the screen, </li><li> all white pixels of the monitor are located on the frame, </li><li> of all frames that satisfy the previous three conditions, the required frame must have the smallest size. </li></ul><p>Formally, a square frame is represented by such pixels of the solid square, that are on the square's border, that is, are not fully surrounded by the other pixels of the square. For example, if the frame's size is <span class="tex-span"><i>d</i> = 3</span>, then it consists of 8 pixels, if its size is <span class="tex-span"><i>d</i> = 2</span>, then it contains 4 pixels and if <span class="tex-span"><i>d</i> = 1</span>, then the frame is reduced to a single pixel.</p></div><div class="input-specification"><p>The first line contains the resolution of the monitor as a pair of integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 2000</span>). The next <span class="tex-span"><i>n</i></span> lines contain exactly <span class="tex-span"><i>m</i></span> characters each — the state of the monitor pixels at the moment of the game. Character "<span class="tex-font-style-tt">.</span>" (period, ASCII code 46) corresponds to the black pixel, and character "<span class="tex-font-style-tt">w</span>" (lowercase English letter <span class="tex-font-style-tt">w</span>) corresponds to the white pixel. It is guaranteed that at least one pixel of the monitor is white.</p></div><div class="output-specification"><p>Print the monitor screen. Represent the sought frame by characters "<span class="tex-font-style-tt">+</span>" (the "plus" character). The pixels that has become white during the game mustn't be changed. Print them as "<span class="tex-font-style-tt">w</span>". If there are multiple possible ways to position the frame of the minimum size, print any of them.</p><p>If the required frame doesn't exist, then print a single line containing number <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains the resolution of the monitor as a pair of integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 2000</span>). The next <span class="tex-span"><i>n</i></span> lines contain exactly <span class="tex-span"><i>m</i></span> characters each — the state of the monitor pixels at the moment of the game. Character "<span class="tex-font-style-tt">.</span>" (period, ASCII code 46) corresponds to the black pixel, and character "<span class="tex-font-style-tt">w</span>" (lowercase English letter <span class="tex-font-style-tt">w</span>) corresponds to the white pixel. It is guaranteed that at least one pixel of the monitor is white.</p>

## Output

<p>Print the monitor screen. Represent the sought frame by characters "<span class="tex-font-style-tt">+</span>" (the "plus" character). The pixels that has become white during the game mustn't be changed. Print them as "<span class="tex-font-style-tt">w</span>". If there are multiple possible ways to position the frame of the minimum size, print any of them.</p><p>If the required frame doesn't exist, then print a single line containing number <span class="tex-font-style-tt">-1</span>.</p>





```input1
4 8
..w..w..
........
........
..w..w..

```




```input2
5 6
......
.w....
......
..w...
......

```




```input3
2 4
....
.w..

```




```input4
2 6
w..w.w
...w..

```




```output1
..w++w..
..+..+..
..+..+..
..w++w..

```




```output2
......
+w+...
+.+...
++w...
......

```




```output3
....
.w..

```




```output4
-1

```



## Note

<p>In the first sample the required size of the optimal frame equals 4. In the second sample the size of the optimal frame equals 3. In the third sample, the size of the optimal frame is 1. In the fourth sample, the required frame doesn't exist.</p>
