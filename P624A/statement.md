## Description

<div><p>Luke Skywalker got locked up in a rubbish shredder between two presses. R2D2 is already working on his rescue, but Luke needs to stay alive as long as possible. For simplicity we will assume that everything happens on a straight line, the presses are initially at coordinates <span class="tex-span">0</span> and <span class="tex-span"><i>L</i></span>, and they move towards each other with speed <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span>, respectively. Luke has width <span class="tex-span"><i>d</i></span> and is able to choose any position between the presses. Luke dies as soon as the distance between the presses is less than his width. Your task is to determine for how long Luke can stay alive.</p></div><div class="input-specification"><p>The first line of the input contains four integers <span class="tex-span"><i>d</i></span>, <span class="tex-span"><i>L</i></span>, <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>d</i>, <i>L</i>, <i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub> ≤ 10 000, <i>d</i> &lt; <i>L</i></span>)&nbsp;— Luke's width, the initial position of the second press and the speed of the first and second presses, respectively.</p></div><div class="output-specification"><p>Print a single real value&nbsp;— the maximum period of time Luke can stay alive for. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://tk7rUXuD.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line of the input contains four integers <span class="tex-span"><i>d</i></span>, <span class="tex-span"><i>L</i></span>, <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>d</i>, <i>L</i>, <i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub> ≤ 10 000, <i>d</i> &lt; <i>L</i></span>)&nbsp;— Luke's width, the initial position of the second press and the speed of the first and second presses, respectively.</p>

## Output

<p>Print a single real value&nbsp;— the maximum period of time Luke can stay alive for. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://tk7rUXuD.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
2 6 2 2

```




```input2
1 9 1 2

```




```output1
1.00000000000000000000

```




```output2
2.66666666666666650000

```



## Note

<p>In the first sample Luke should stay exactly in the middle of the segment, that is at coordinates <span class="tex-span">[2;4]</span>, as the presses move with the same speed.</p><p>In the second sample he needs to occupy the position <img align="middle" class="tex-formula" src="file://LTwT2huN.png" style="max-width: 100.0%;max-height: 100.0%;">. In this case both presses move to his edges at the same time.</p>
