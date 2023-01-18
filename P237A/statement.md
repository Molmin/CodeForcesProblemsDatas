## Description

<div><p>Valera runs a 24/7 fast food cafe. He magically learned that next day <span class="tex-span"><i>n</i></span> people will visit his cafe. For each person we know the arrival time: the <span class="tex-span"><i>i</i></span>-th person comes exactly at <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> hours <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> minutes. The cafe spends less than a minute to serve each client, but if a client comes in and sees that there is no free cash, than he doesn't want to wait and leaves the cafe immediately. </p><p>Valera is very greedy, so he wants to serve all <span class="tex-span"><i>n</i></span> customers next day (and get more profit). However, for that he needs to ensure that at each moment of time the number of working cashes is no less than the number of clients in the cafe. </p><p>Help Valera count the minimum number of cashes to work at his cafe next day, so that they can serve all visitors.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>, that is the number of cafe visitors.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines has two space-separated integers <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 23;&nbsp;0 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ 59)</span>, representing the time when the <span class="tex-span"><i>i</i></span>-th person comes into the cafe. </p><p>Note that the time is given in the <span class="tex-font-style-bf">chronological</span> order. All time is given within one 24-hour period.</p></div><div class="output-specification"><p>Print a single integer — the minimum number of cashes, needed to serve all clients next day.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>, that is the number of cafe visitors.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines has two space-separated integers <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 23;&nbsp;0 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ 59)</span>, representing the time when the <span class="tex-span"><i>i</i></span>-th person comes into the cafe. </p><p>Note that the time is given in the <span class="tex-font-style-bf">chronological</span> order. All time is given within one 24-hour period.</p>

## Output

<p>Print a single integer — the minimum number of cashes, needed to serve all clients next day.</p>





```input1
4
8 0
8 10
8 10
8 45

```




```input2
3
0 12
10 11
22 22

```




```output1
2

```




```output2
1

```



## Note

<p>In the first sample it is not enough one cash to serve all clients, because two visitors will come into cafe in 8:10. Therefore, if there will be one cash in cafe, then one customer will be served by it, and another one will not wait and will go away.</p><p>In the second sample all visitors will come in different times, so it will be enough one cash.</p>
