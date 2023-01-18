## Description

<div><p>Bear Limak likes watching sports on TV. He is going to watch a game today. The game lasts <span class="tex-span">90</span> minutes and there are no breaks.</p><p>Each minute can be either interesting or boring. If <span class="tex-span">15</span> consecutive minutes are boring then Limak immediately turns TV off.</p><p>You know that there will be <span class="tex-span"><i>n</i></span> interesting minutes <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span>. Your task is to calculate for how many minutes Limak will watch the game.</p></div><div class="input-specification"><p>The first line of the input contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 90</span>)&nbsp;— the number of interesting minutes.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index">1</sub> &lt; <i>t</i><sub class="lower-index">2</sub> &lt; ... <i>t</i><sub class="lower-index"><i>n</i></sub> ≤ 90</span>), given in the increasing order.</p></div><div class="output-specification"><p>Print the number of minutes Limak will watch the game.</p></div>

## Input

<p>The first line of the input contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 90</span>)&nbsp;— the number of interesting minutes.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index">1</sub> &lt; <i>t</i><sub class="lower-index">2</sub> &lt; ... <i>t</i><sub class="lower-index"><i>n</i></sub> ≤ 90</span>), given in the increasing order.</p>

## Output

<p>Print the number of minutes Limak will watch the game.</p>





```input1
3
7 20 88

```




```input2
9
16 20 30 40 50 60 70 80 90

```




```input3
9
15 20 30 40 50 60 70 80 90

```




```output1
35

```




```output2
15

```




```output3
90

```



## Note

<p>In the first sample, minutes <span class="tex-span">21, 22, ..., 35</span> are all boring and thus Limak will turn TV off immediately after the <span class="tex-span">35</span>-th minute. So, he would watch the game for <span class="tex-span">35</span> minutes.</p><p>In the second sample, the first <span class="tex-span">15</span> minutes are boring.</p><p>In the third sample, there are no consecutive <span class="tex-span">15</span> boring minutes. So, Limak will watch the whole game.</p>
