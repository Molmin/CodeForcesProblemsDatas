## Description

<div><p>Consider <span class="tex-span">2<i>n</i></span> rows of the seats in a bus. <span class="tex-span"><i>n</i></span> rows of the seats on the left and <span class="tex-span"><i>n</i></span> rows of the seats on the right. Each row can be filled by two people. So the total capacity of the bus is <span class="tex-span">4<i>n</i></span>.</p><p>Consider that <span class="tex-span"><i>m</i></span> (<span class="tex-span"><i>m</i> ≤ 4<i>n</i></span>) people occupy the seats in the bus. The passengers entering the bus are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> (in the order of their entering the bus). The pattern of the seat occupation is as below:</p><p><span class="tex-span">1</span>-st row left window seat, <span class="tex-span">1</span>-st row right window seat, <span class="tex-span">2</span>-nd row left window seat, <span class="tex-span">2</span>-nd row right window seat, ... , <span class="tex-span"><i>n</i></span>-th row left window seat, <span class="tex-span"><i>n</i></span>-th row right window seat.</p><p>After occupying all the window seats (for <span class="tex-span"><i>m</i> &gt; 2<i>n</i></span>) the non-window seats are occupied:</p><p><span class="tex-span">1</span>-st row left non-window seat, <span class="tex-span">1</span>-st row right non-window seat, ... , <span class="tex-span"><i>n</i></span>-th row left non-window seat, <span class="tex-span"><i>n</i></span>-th row right non-window seat.</p><p>All the passengers go to a single final destination. In the final destination, the passengers get off in the given order.</p><p><span class="tex-span">1</span>-st row left non-window seat, <span class="tex-span">1</span>-st row left window seat, <span class="tex-span">1</span>-st row right non-window seat, <span class="tex-span">1</span>-st row right window seat, ... , <span class="tex-span"><i>n</i></span>-th row left non-window seat, <span class="tex-span"><i>n</i></span>-th row left window seat, <span class="tex-span"><i>n</i></span>-th row right non-window seat, <span class="tex-span"><i>n</i></span>-th row right window seat.</p><center> <img class="tex-graphics" src="file://ID8UlYaQ.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">The seating for <span class="tex-span"><i>n</i> = 9</span> and <span class="tex-span"><i>m</i> = 36</span>.</span> </center><p>You are given the values <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>. Output <span class="tex-span"><i>m</i></span> numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>, the order in which the passengers will get off the bus.</p></div><div class="input-specification"><p>The only line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100, 1 ≤ <i>m</i> ≤ 4<i>n</i></span>) — the number of pairs of rows and the number of passengers.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> distinct integers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> — the order in which the passengers will get off the bus.</p></div>

## Input

<p>The only line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100, 1 ≤ <i>m</i> ≤ 4<i>n</i></span>) — the number of pairs of rows and the number of passengers.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> distinct integers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> — the order in which the passengers will get off the bus.</p>





```input1
2 7

```




```input2
9 36

```




```output1
5 1 6 2 7 3 4

```




```output2
19 1 20 2 21 3 22 4 23 5 24 6 25 7 26 8 27 9 28 10 29 11 30 12 31 13 32 14 33 15 34 16 35 17 36 18

```


