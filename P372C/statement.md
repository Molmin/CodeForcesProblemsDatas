## Description

<div><p>A festival will be held in a town's main street. There are <span class="tex-span"><i>n</i></span> sections in the main street. The sections are numbered <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span> from left to right. The distance between each adjacent sections is <span class="tex-span">1</span>.</p><p>In the festival <span class="tex-span"><i>m</i></span> fireworks will be launched. The <span class="tex-span"><i>i</i></span>-th (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>m</i></span>) launching is on time <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> at section <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. If you are at section <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span>) at the time of <span class="tex-span"><i>i</i></span>-th launching, you'll gain happiness value <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> - |<i>a</i><sub class="lower-index"><i>i</i></sub> - <i>x</i>|</span> (note that the happiness value might be a negative value).</p><p>You can move up to <span class="tex-span"><i>d</i></span> length units in a unit time interval, but it's prohibited to go out of the main street. Also you can be in an arbitrary section at initial time moment (time equals to <span class="tex-span">1</span>), and want to maximize the sum of happiness that can be gained from watching fireworks. Find the maximum total happiness.</p><p>Note that two or more fireworks can be launched at the same time.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 150000;&nbsp;1 ≤ <i>m</i> ≤ 300;&nbsp;1 ≤ <i>d</i> ≤ <i>n</i></span>).</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>;&nbsp;1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). The <span class="tex-span"><i>i</i></span>-th line contains description of the <span class="tex-span"><i>i</i></span>-th launching.</p><p>It is guaranteed that the condition <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> ≤ <i>t</i><sub class="lower-index"><i>i</i> + 1</sub></span> (<span class="tex-span">1 ≤ <i>i</i> &lt; <i>m</i></span>) will be satisfied.</p></div><div class="output-specification"><p>Print a single integer — the maximum sum of happiness that you can gain from watching all the fireworks.</p><p>Please, do not write the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in C++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 150000;&nbsp;1 ≤ <i>m</i> ≤ 300;&nbsp;1 ≤ <i>d</i> ≤ <i>n</i></span>).</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>;&nbsp;1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). The <span class="tex-span"><i>i</i></span>-th line contains description of the <span class="tex-span"><i>i</i></span>-th launching.</p><p>It is guaranteed that the condition <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> ≤ <i>t</i><sub class="lower-index"><i>i</i> + 1</sub></span> (<span class="tex-span">1 ≤ <i>i</i> &lt; <i>m</i></span>) will be satisfied.</p>

## Output

<p>Print a single integer — the maximum sum of happiness that you can gain from watching all the fireworks.</p><p>Please, do not write the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in C++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
50 3 1
49 1 1
26 1 4
6 1 10

```




```input2
10 2 1
1 1000 4
9 1000 4

```




```output1
-31

```




```output2
1992

```


