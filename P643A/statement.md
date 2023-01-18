## Description

<div><p>Bear Limak has <span class="tex-span"><i>n</i></span> colored balls, arranged in one long row. Balls are numbered <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span>, from left to right. There are <span class="tex-span"><i>n</i></span> possible colors, also numbered <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span>. The <span class="tex-span"><i>i</i></span>-th ball has color <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>For a fixed interval (set of consecutive elements) of balls we can define a <span class="tex-font-style-it">dominant</span> color. It's a color occurring the biggest number of times in the interval. In case of a tie between some colors, the one with the smallest number (index) is chosen as dominant.</p><p>There are <img align="middle" class="tex-formula" src="file://gPFrwVxM.png" style="max-width: 100.0%;max-height: 100.0%;"> non-empty intervals in total. For each color, your task is to count the number of intervals in which this color is dominant.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>)&nbsp;— the number of balls.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is the color of the <span class="tex-span"><i>i</i></span>-th ball.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> integers. The <span class="tex-span"><i>i</i></span>-th of them should be equal to the number of intervals where <span class="tex-span"><i>i</i></span> is a dominant color.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>)&nbsp;— the number of balls.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is the color of the <span class="tex-span"><i>i</i></span>-th ball.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> integers. The <span class="tex-span"><i>i</i></span>-th of them should be equal to the number of intervals where <span class="tex-span"><i>i</i></span> is a dominant color.</p>





```input1
4
1 2 1 2

```




```input2
3
1 1 1

```




```output1
7 3 0 0 

```




```output2
6 0 0 

```



## Note

<p>In the first sample, color <span class="tex-span">2</span> is dominant in three intervals:</p><ul> <li> An interval <span class="tex-span">[2, 2]</span> contains one ball. This ball's color is <span class="tex-span">2</span> so it's clearly a dominant color. </li><li> An interval <span class="tex-span">[4, 4]</span> contains one ball, with color <span class="tex-span">2</span> again. </li><li> An interval <span class="tex-span">[2, 4]</span> contains two balls of color <span class="tex-span">2</span> and one ball of color <span class="tex-span">1</span>. </li></ul><p>There are <span class="tex-span">7</span> more intervals and color <span class="tex-span">1</span> is dominant in all of them.</p>
