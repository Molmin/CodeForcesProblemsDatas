## Description

<div><p>The Berland Armed Forces System consists of <span class="tex-span"><i>n</i></span> ranks that are numbered using natural numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, where <span class="tex-span">1</span> is the lowest rank and <span class="tex-span"><i>n</i></span> is the highest rank.</p><p>One needs exactly <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> years to rise from rank <span class="tex-span"><i>i</i></span> to rank <span class="tex-span"><i>i</i> + 1</span>. Reaching a certain rank <span class="tex-span"><i>i</i></span> having not reached all the previous <span class="tex-span"><i>i</i> - 1</span> ranks is impossible.</p><p>Vasya has just reached a new rank of <span class="tex-span"><i>a</i></span>, but he dreams of holding the rank of <span class="tex-span"><i>b</i></span>. Find for how many more years Vasya should serve in the army until he can finally realize his dream.</p></div><div class="input-specification"><p>The first input line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>). The second line contains <span class="tex-span"><i>n</i> - 1</span> integers <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>). The third input line contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i> &lt; <i>b</i> ≤ <i>n</i></span>). The numbers on the lines are space-separated.</p></div><div class="output-specification"><p>Print the single number which is the number of years that Vasya needs to rise from rank <span class="tex-span"><i>a</i></span> to rank <span class="tex-span"><i>b</i></span>.</p></div>

## Input

<p>The first input line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>). The second line contains <span class="tex-span"><i>n</i> - 1</span> integers <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>). The third input line contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i> &lt; <i>b</i> ≤ <i>n</i></span>). The numbers on the lines are space-separated.</p>

## Output

<p>Print the single number which is the number of years that Vasya needs to rise from rank <span class="tex-span"><i>a</i></span> to rank <span class="tex-span"><i>b</i></span>.</p>





```input1
3
5 6
1 2

```




```input2
3
5 6
1 3

```




```output1
5

```




```output2
11

```


