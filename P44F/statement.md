## Description

<div><p>Anfisa the monkey got disappointed in word processors as they aren't good enough at reflecting all the range of her emotions, that's why she decided to switch to graphics editors. Having opened the BerPaint, she saw a white rectangle <span class="tex-span"><i>W</i> × <i>H</i></span> in size which can be painted on. First Anfisa learnt to navigate the drawing tool which is used to paint segments and quickly painted on that rectangle a certain number of black-colored segments. The resulting picture didn't seem bright enough to Anfisa, that's why she turned her attention to the "fill" tool which is used to find a point on the rectangle to paint and choose a color, after which all the area which is the same color as the point it contains, is completely painted the chosen color. Having applied the fill several times, Anfisa expressed her emotions completely and stopped painting. Your task is by the information on the painted segments and applied fills to find out for every color the total area of the areas painted this color after all the fills.</p></div><div class="input-specification"><p>The first input line has two integers <span class="tex-span"><i>W</i></span> and <span class="tex-span"><i>H</i></span> (<span class="tex-span">3 ≤ <i>W</i>, <i>H</i> ≤ 10<sup class="upper-index">4</sup></span>) — the sizes of the initially white rectangular painting area. The second line contains integer <span class="tex-span"><i>n</i></span> — the number of black segments (<span class="tex-span">0 ≤ <i>n</i> ≤ 100</span>). On the next <span class="tex-span"><i>n</i></span> lines are described the segments themselves, each of which is given by coordinates of their endpoints <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">0 &lt; <i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub> &lt; <i>W</i>, 0 &lt; <i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub> &lt; <i>H</i></span>). All segments have non-zero length. The next line contains preset number of fills <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>m</i> ≤ 100</span>). Each of the following <span class="tex-span"><i>m</i></span> lines defines the fill operation in the form of "<span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span> <span class="tex-span"><i>color</i></span>", where <span class="tex-span">(<i>x</i>, <i>y</i>)</span> are the coordinates of the chosen point (<span class="tex-span">0 &lt; <i>x</i> &lt; <i>W</i>, 0 &lt; <i>y</i> &lt; <i>H</i></span>), and <span class="tex-span"><i>color</i></span> — a line of lowercase Latin letters from 1 to 15 symbols in length, determining the color. All coordinates given in the input are integers. Initially the rectangle is "white" in color, whereas the segments are drawn "black" in color.</p></div><div class="output-specification"><p>For every color present in the final picture print on the single line the name of the color and the total area of areas painted that color with an accuracy of <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. Print the colors in any order. </p></div>

## Input

<p>The first input line has two integers <span class="tex-span"><i>W</i></span> and <span class="tex-span"><i>H</i></span> (<span class="tex-span">3 ≤ <i>W</i>, <i>H</i> ≤ 10<sup class="upper-index">4</sup></span>) — the sizes of the initially white rectangular painting area. The second line contains integer <span class="tex-span"><i>n</i></span> — the number of black segments (<span class="tex-span">0 ≤ <i>n</i> ≤ 100</span>). On the next <span class="tex-span"><i>n</i></span> lines are described the segments themselves, each of which is given by coordinates of their endpoints <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">0 &lt; <i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub> &lt; <i>W</i>, 0 &lt; <i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub> &lt; <i>H</i></span>). All segments have non-zero length. The next line contains preset number of fills <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>m</i> ≤ 100</span>). Each of the following <span class="tex-span"><i>m</i></span> lines defines the fill operation in the form of "<span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span> <span class="tex-span"><i>color</i></span>", where <span class="tex-span">(<i>x</i>, <i>y</i>)</span> are the coordinates of the chosen point (<span class="tex-span">0 &lt; <i>x</i> &lt; <i>W</i>, 0 &lt; <i>y</i> &lt; <i>H</i></span>), and <span class="tex-span"><i>color</i></span> — a line of lowercase Latin letters from 1 to 15 symbols in length, determining the color. All coordinates given in the input are integers. Initially the rectangle is "white" in color, whereas the segments are drawn "black" in color.</p>

## Output

<p>For every color present in the final picture print on the single line the name of the color and the total area of areas painted that color with an accuracy of <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. Print the colors in any order. </p>





```input1
4 5
6
1 1 1 3
1 3 3 3
3 3 3 1
3 1 1 1
1 3 3 1
1 1 3 3
2
2 1 red
2 2 blue

```




```input2
5 5
5
1 1 2 2
2 2 4 2
4 2 4 4
4 4 2 4
2 4 2 2
2
3 3 black
3 3 green

```




```input3
7 4
9
1 2 2 3
2 3 3 2
3 2 2 1
2 1 1 2
3 2 4 2
4 2 5 3
5 3 6 2
6 2 5 1
5 1 4 2
2
2 2 black
2 2 red

```




```output1
blue 0.00000000
white 20.00000000

```




```output2
green 4.00000000
white 21.00000000

```




```output3
red 2.00000000
white 26.00000000

```



## Note

<p>Initially the black segments painted by Anfisa can also be painted a color if any of the chosen points lays on the segment. The segments have areas equal to 0. That is why if in the final picture only parts of segments is painted some color, then the area, painted the color is equal to 0.</p>
