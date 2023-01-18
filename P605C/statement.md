## Description

<div><p>Mikhail the Freelancer dreams of two things: to become a cool programmer and to buy a flat in Moscow. To become a cool programmer, he needs at least <span class="tex-span"><i>p</i></span> experience points, and a desired flat in Moscow costs <span class="tex-span"><i>q</i></span> dollars. Mikhail is determined to follow his dreams and registered at a freelance site.</p><p>He has suggestions to work on <span class="tex-span"><i>n</i></span> distinct projects. Mikhail has already evaluated that the participation in the <span class="tex-span"><i>i</i></span>-th project will increase his experience by <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> per day and bring <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> dollars per day. As freelance work implies flexible working hours, Mikhail is free to stop working on one project at any time and start working on another project. Doing so, he receives the respective share of experience and money. Mikhail is only trying to become a cool programmer, so he is able to work only on one project at any moment of time.</p><p>Find the real value, equal to the minimum number of days Mikhail needs to make his dream come true.</p><p>For example, suppose Mikhail is suggested to work on three projects and <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> = 6</span>, <span class="tex-span"><i>b</i><sub class="lower-index">1</sub> = 2</span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub> = 1</span>, <span class="tex-span"><i>b</i><sub class="lower-index">2</sub> = 3</span>, <span class="tex-span"><i>a</i><sub class="lower-index">3</sub> = 2</span>, <span class="tex-span"><i>b</i><sub class="lower-index">3</sub> = 6</span>. Also, <span class="tex-span"><i>p</i> = 20</span> and <span class="tex-span"><i>q</i> = 20</span>. In order to achieve his aims Mikhail has to work for <span class="tex-span">2.5</span> days on both first and third projects. Indeed, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>·2.5 + <i>a</i><sub class="lower-index">2</sub>·0 + <i>a</i><sub class="lower-index">3</sub>·2.5 = 6·2.5 + 1·0 + 2·2.5 = 20</span> and <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>·2.5 + <i>b</i><sub class="lower-index">2</sub>·0 + <i>b</i><sub class="lower-index">3</sub>·2.5 = 2·2.5 + 3·0 + 6·2.5 = 20</span>.</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000, 1 ≤ <i>p</i>, <i>q</i> ≤ 1 000 000</span>)&nbsp;— the number of projects and the required number of experience and money.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>)&nbsp;— the daily increase in experience and daily income for working on the <span class="tex-span"><i>i</i></span>-th project.</p></div><div class="output-specification"><p>Print a real value&nbsp;— the minimum number of days Mikhail needs to get the required amount of experience and money. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://J61kui2E.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000, 1 ≤ <i>p</i>, <i>q</i> ≤ 1 000 000</span>)&nbsp;— the number of projects and the required number of experience and money.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>)&nbsp;— the daily increase in experience and daily income for working on the <span class="tex-span"><i>i</i></span>-th project.</p>

## Output

<p>Print a real value&nbsp;— the minimum number of days Mikhail needs to get the required amount of experience and money. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://J61kui2E.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
3 20 20
6 2
1 3
2 6

```




```input2
4 1 1
2 3
3 2
2 3
3 2

```




```output1
5.000000000000000

```




```output2
0.400000000000000

```



## Note

<p>First sample corresponds to the example in the problem statement.</p>
