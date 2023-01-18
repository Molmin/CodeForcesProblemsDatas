## Description

<div><p>You are given a figure on a grid representing stairs consisting of 7 steps. The width of the stair on height <span class="tex-span"><i>i</i></span> is <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> squares. Formally, the figure is created by consecutively joining rectangles of size <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub> × <i>i</i></span> so that the <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> sides lie on one straight line. Thus, for example, if all <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub> = 1</span>, the figure will look like that (different colors represent different rectangles):</p><center> <img class="tex-graphics" src="file://qYzMNjrO.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>And if <span class="tex-span"><i>w</i> = {5, 1, 0, 3, 0, 0, 1}</span>, then it looks like that:</p><center> <img class="tex-graphics" src="file://HLrD9LcN.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Find the number of ways to color some borders of the figure's inner squares so that no square had all four borders colored. The borders of the squares lying on the border of the figure should be considered painted. The ways that differ with the figure's rotation should be considered distinct. </p></div><div class="input-specification"><p>The single line of the input contains 7 numbers <span class="tex-span"><i>w</i><sub class="lower-index">1</sub>, <i>w</i><sub class="lower-index">2</sub>, ..., <i>w</i><sub class="lower-index">7</sub></span> (<span class="tex-span">0 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>). It is guaranteed that at least one of the <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>'s isn't equal to zero.</p></div><div class="output-specification"><p>In the single line of the output display a single number — the answer to the problem modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The single line of the input contains 7 numbers <span class="tex-span"><i>w</i><sub class="lower-index">1</sub>, <i>w</i><sub class="lower-index">2</sub>, ..., <i>w</i><sub class="lower-index">7</sub></span> (<span class="tex-span">0 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>). It is guaranteed that at least one of the <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>'s isn't equal to zero.</p>

## Output

<p>In the single line of the output display a single number — the answer to the problem modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
0 1 0 0 0 0 0

```




```input2
0 2 0 0 0 0 0

```




```input3
1 1 1 0 0 0 0

```




```input4
5 1 0 3 0 0 1

```




```output1
1

```




```output2
7

```




```output3
9

```




```output4
411199181

```



## Note

<p>All the possible ways of painting the third sample are given below:</p><center> <img class="tex-graphics" src="file://47WxPzD3.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
