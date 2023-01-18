## Description

<div><p>A well-known art union called "Kalevich is Alive!" manufactures objects d'art (pictures). The union consists of <span class="tex-span"><i>n</i></span> painters who decided to organize their work as follows.</p><p>Each painter uses only the color that was assigned to him. The colors are distinct for all painters. Let's assume that the first painter uses color 1, the second one uses color 2, and so on. Each picture will contain all these <span class="tex-span"><i>n</i></span> colors. Adding the <span class="tex-span"><i>j</i></span>-th color to the <span class="tex-span"><i>i</i></span>-th picture takes the <span class="tex-span"><i>j</i></span>-th painter <span class="tex-span"><i>t</i><sub class="lower-index"><i>ij</i></sub></span> units of time.</p><p>Order is important everywhere, so the painters' work is ordered by the following rules:</p><ul> <li> Each picture is first painted by the first painter, then by the second one, and so on. That is, after the <span class="tex-span"><i>j</i></span>-th painter finishes working on the picture, it must go to the <span class="tex-span">(<i>j</i> + 1)</span>-th painter (if <span class="tex-span"><i>j</i> &lt; <i>n</i></span>); </li><li> each painter works on the pictures in some order: first, he paints the first picture, then he paints the second picture and so on; </li><li> each painter can simultaneously work on at most one picture. However, the painters don't need any time to have a rest; </li><li> as soon as the <span class="tex-span"><i>j</i></span>-th painter finishes his part of working on the picture, the picture immediately becomes available to the next painter. </li></ul><p>Given that the painters start working at time 0, find for each picture the time when it is ready for sale.</p></div><div class="input-specification"><p>The first line of the input contains integers <span class="tex-span"><i>m</i>, <i>n</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 50000, 1 ≤ <i>n</i> ≤ 5</span>), where <span class="tex-span"><i>m</i></span> is the number of pictures and <span class="tex-span"><i>n</i></span> is the number of painters. Then follow the descriptions of the pictures, one per line. Each line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i>1</sub>, <i>t</i><sub class="lower-index"><i>i</i>2</sub>, ..., <i>t</i><sub class="lower-index"><i>in</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>ij</i></sub> ≤ 1000</span>), where <span class="tex-span"><i>t</i><sub class="lower-index"><i>ij</i></sub></span> is the time the <span class="tex-span"><i>j</i></span>-th painter needs to work on the <span class="tex-span"><i>i</i></span>-th picture.</p></div><div class="output-specification"><p>Print the sequence of <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>r</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub>, ..., <i>r</i><sub class="lower-index"><i>m</i></sub></span>, where <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> is the moment when the <span class="tex-span"><i>n</i></span>-th painter stopped working on the <span class="tex-span"><i>i</i></span>-th picture.</p></div>

## Input

<p>The first line of the input contains integers <span class="tex-span"><i>m</i>, <i>n</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 50000, 1 ≤ <i>n</i> ≤ 5</span>), where <span class="tex-span"><i>m</i></span> is the number of pictures and <span class="tex-span"><i>n</i></span> is the number of painters. Then follow the descriptions of the pictures, one per line. Each line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i>1</sub>, <i>t</i><sub class="lower-index"><i>i</i>2</sub>, ..., <i>t</i><sub class="lower-index"><i>in</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>ij</i></sub> ≤ 1000</span>), where <span class="tex-span"><i>t</i><sub class="lower-index"><i>ij</i></sub></span> is the time the <span class="tex-span"><i>j</i></span>-th painter needs to work on the <span class="tex-span"><i>i</i></span>-th picture.</p>

## Output

<p>Print the sequence of <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>r</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub>, ..., <i>r</i><sub class="lower-index"><i>m</i></sub></span>, where <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> is the moment when the <span class="tex-span"><i>n</i></span>-th painter stopped working on the <span class="tex-span"><i>i</i></span>-th picture.</p>





```input1
5 1
1
2
3
4
5

```




```input2
4 2
2 5
3 1
5 3
10 1

```




```output1
1 3 6 10 15
```




```output2
7 8 13 21
```


