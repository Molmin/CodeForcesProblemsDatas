## Description

<div><p>Recently Luba bought a very interesting book. She knows that it will take <span class="tex-span"><i>t</i></span> seconds to read the book. Luba wants to finish reading as fast as she can.</p><p>But she has some work to do in each of <span class="tex-span"><i>n</i></span> next days. The number of seconds that Luba has to spend working during <span class="tex-span"><i>i</i></span>-th day is <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. If some free time remains, she can spend it on reading.</p><p>Help Luba to determine the minimum number of day when she finishes reading.</p><p><span class="tex-font-style-bf">It is guaranteed that the answer doesn't exceed <span class="tex-span"><i>n</i></span>.</span></p><p><span class="tex-font-style-bf">Remember that there are 86400 seconds in a day.</span></p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>t</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of days and the time required to read the book.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 86400</span>) — the time Luba has to spend on her work during <span class="tex-span"><i>i</i></span>-th day.</p></div><div class="output-specification"><p>Print the minimum day Luba can finish reading the book.</p><p><span class="tex-font-style-bf">It is guaranteed that answer doesn't exceed <span class="tex-span"><i>n</i></span></span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>t</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of days and the time required to read the book.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 86400</span>) — the time Luba has to spend on her work during <span class="tex-span"><i>i</i></span>-th day.</p>

## Output

<p>Print the minimum day Luba can finish reading the book.</p><p><span class="tex-font-style-bf">It is guaranteed that answer doesn't exceed <span class="tex-span"><i>n</i></span></span>.</p>





```input1
2 2
86400 86398

```




```input2
2 86400
0 86400

```




```output1
2

```




```output2
1

```


