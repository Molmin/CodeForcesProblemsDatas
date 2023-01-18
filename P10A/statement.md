## Description

<div><p>Tom is interested in power consumption of his favourite laptop. His laptop has three modes. In normal mode laptop consumes <span class="tex-span"><i>P</i><sub class="lower-index">1</sub></span> watt per minute. <span class="tex-span"><i>T</i><sub class="lower-index">1</sub></span> minutes after Tom moved the mouse or touched the keyboard for the last time, a screensaver starts and power consumption changes to <span class="tex-span"><i>P</i><sub class="lower-index">2</sub></span> watt per minute. Finally, after <span class="tex-span"><i>T</i><sub class="lower-index">2</sub></span> minutes from the start of the screensaver, laptop switches to the "sleep" mode and consumes <span class="tex-span"><i>P</i><sub class="lower-index">3</sub></span> watt per minute. If Tom moves the mouse or touches the keyboard when the laptop is in the second or in the third mode, it switches to the first (normal) mode. Tom's work with the laptop can be divided into <span class="tex-span"><i>n</i></span> time periods <span class="tex-span">[<i>l</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">1</sub>], [<i>l</i><sub class="lower-index">2</sub>, <i>r</i><sub class="lower-index">2</sub>], ..., [<i>l</i><sub class="lower-index"><i>n</i></sub>, <i>r</i><sub class="lower-index"><i>n</i></sub>]</span>. During each interval Tom continuously moves the mouse and presses buttons on the keyboard. Between the periods Tom stays away from the laptop. Find out the total amount of power consumed by the laptop during the period <span class="tex-span">[<i>l</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index"><i>n</i></sub>]</span>.</p></div><div class="input-specification"><p>The first line contains 6 integer numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>P</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>P</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>P</i><sub class="lower-index">3</sub></span>, <span class="tex-span"><i>T</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>T</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100, 0 ≤ <i>P</i><sub class="lower-index">1</sub>, <i>P</i><sub class="lower-index">2</sub>, <i>P</i><sub class="lower-index">3</sub> ≤ 100, 1 ≤ <i>T</i><sub class="lower-index">1</sub>, <i>T</i><sub class="lower-index">2</sub> ≤ 60</span>). The following <span class="tex-span"><i>n</i></span> lines contain description of Tom's work. Each <span class="tex-span"><i>i</i></span>-th of these lines contains two space-separated integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 1440</span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub> &lt; <i>l</i><sub class="lower-index"><i>i</i> + 1</sub></span> for <span class="tex-span"><i>i</i> &lt; <i>n</i></span>), which stand for the start and the end of the <span class="tex-span"><i>i</i></span>-th period of work.</p></div><div class="output-specification"><p>Output the answer to the problem.</p></div>

## Input

<p>The first line contains 6 integer numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>P</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>P</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>P</i><sub class="lower-index">3</sub></span>, <span class="tex-span"><i>T</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>T</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100, 0 ≤ <i>P</i><sub class="lower-index">1</sub>, <i>P</i><sub class="lower-index">2</sub>, <i>P</i><sub class="lower-index">3</sub> ≤ 100, 1 ≤ <i>T</i><sub class="lower-index">1</sub>, <i>T</i><sub class="lower-index">2</sub> ≤ 60</span>). The following <span class="tex-span"><i>n</i></span> lines contain description of Tom's work. Each <span class="tex-span"><i>i</i></span>-th of these lines contains two space-separated integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 1440</span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub> &lt; <i>l</i><sub class="lower-index"><i>i</i> + 1</sub></span> for <span class="tex-span"><i>i</i> &lt; <i>n</i></span>), which stand for the start and the end of the <span class="tex-span"><i>i</i></span>-th period of work.</p>

## Output

<p>Output the answer to the problem.</p>





```input1
1 3 2 1 5 10
0 10

```




```input2
2 8 4 2 5 10
20 30
50 100

```




```output1
30
```




```output2
570
```


