## Description

<div><p>On a history lesson the teacher asked Vasya to name the dates when <span class="tex-span"><i>n</i></span> famous events took place. He doesn't remembers the exact dates but he remembers a segment of days <span class="tex-span">[<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>]</span> (inclusive) on which the event could have taken place. However Vasya also remembers that there was at most one event in one day. Help him choose such <span class="tex-span"><i>n</i></span> dates of famous events that will fulfill both conditions. It is guaranteed that it is possible.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of known events. Then follow <span class="tex-span"><i>n</i></span> lines containing two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> each (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>) — the earliest acceptable date and the latest acceptable date of the <span class="tex-span"><i>i</i></span>-th event.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> numbers — the dates on which the events took place. If there are several solutions, print any of them. It is guaranteed that a solution exists.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of known events. Then follow <span class="tex-span"><i>n</i></span> lines containing two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> each (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>) — the earliest acceptable date and the latest acceptable date of the <span class="tex-span"><i>i</i></span>-th event.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> numbers — the dates on which the events took place. If there are several solutions, print any of them. It is guaranteed that a solution exists.</p>





```input1
3
1 2
2 3
3 4

```




```input2
2
1 3
1 3

```




```output1
1 2 3 

```




```output2
1 2 

```


