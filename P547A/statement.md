## Description

<div><p>Mike has a frog and a flower. His frog is named Xaniar and his flower is named Abol. Initially(at time <span class="tex-span">0</span>), height of Xaniar is <span class="tex-span"><i>h</i><sub class="lower-index">1</sub></span> and height of Abol is <span class="tex-span"><i>h</i><sub class="lower-index">2</sub></span>. Each second, Mike waters Abol and Xaniar.</p><center> <img class="tex-graphics" src="file://zxyjpZ5p.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>So, if height of Xaniar is <span class="tex-span"><i>h</i><sub class="lower-index">1</sub></span> and height of Abol is <span class="tex-span"><i>h</i><sub class="lower-index">2</sub></span>, after one second height of Xaniar will become <img align="middle" class="tex-formula" src="file://eYS3Ezck.png" style="max-width: 100.0%;max-height: 100.0%;"> and height of Abol will become <img align="middle" class="tex-formula" src="file://GVd0RnkR.png" style="max-width: 100.0%;max-height: 100.0%;"> where <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> are some integer numbers and <img align="middle" class="tex-formula" src="file://VbzLH1De.png" style="max-width: 100.0%;max-height: 100.0%;"> denotes the remainder of <span class="tex-span"><i>a</i></span> modulo <span class="tex-span"><i>b</i></span>.</p><p>Mike is a competitive programmer fan. He wants to know the minimum time it takes until height of Xania is <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> and height of Abol is <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>.</p><p>Mike has asked you for your help. Calculate the minimum time or say it will never happen.</p></div><div class="input-specification"><p>The first line of input contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>).</p><p>The second line of input contains integers <span class="tex-span"><i>h</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> (<span class="tex-span">0 ≤ <i>h</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">1</sub> &lt; <i>m</i></span>).</p><p>The third line of input contains integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub> &lt; <i>m</i></span>).</p><p>The fourth line of input contains integers <span class="tex-span"><i>h</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span> (<span class="tex-span">0 ≤ <i>h</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">2</sub> &lt; <i>m</i></span>).</p><p>The fifth line of input contains integers <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub> &lt; <i>m</i></span>).</p><p>It is guaranteed that <span class="tex-span"><i>h</i><sub class="lower-index">1</sub> ≠ <i>a</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>h</i><sub class="lower-index">2</sub> ≠ <i>a</i><sub class="lower-index">2</sub></span>.</p></div><div class="output-specification"><p>Print the minimum number of seconds until Xaniar reaches height <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> and Abol reaches height <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span> or print -1 otherwise.</p></div>

## Input

<p>The first line of input contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>).</p><p>The second line of input contains integers <span class="tex-span"><i>h</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> (<span class="tex-span">0 ≤ <i>h</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">1</sub> &lt; <i>m</i></span>).</p><p>The third line of input contains integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub> &lt; <i>m</i></span>).</p><p>The fourth line of input contains integers <span class="tex-span"><i>h</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span> (<span class="tex-span">0 ≤ <i>h</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">2</sub> &lt; <i>m</i></span>).</p><p>The fifth line of input contains integers <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub> &lt; <i>m</i></span>).</p><p>It is guaranteed that <span class="tex-span"><i>h</i><sub class="lower-index">1</sub> ≠ <i>a</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>h</i><sub class="lower-index">2</sub> ≠ <i>a</i><sub class="lower-index">2</sub></span>.</p>

## Output

<p>Print the minimum number of seconds until Xaniar reaches height <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> and Abol reaches height <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span> or print -1 otherwise.</p>





```input1
5
4 2
1 1
0 1
2 3

```




```input2
1023
1 2
1 0
1 2
1 1

```




```output1
3

```




```output2
-1

```



## Note

<p>In the first sample, heights sequences are following:</p><p>Xaniar: <img align="middle" class="tex-formula" src="file://wDVOdUgo.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Abol: <img align="middle" class="tex-formula" src="file://FKw01SN3.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
