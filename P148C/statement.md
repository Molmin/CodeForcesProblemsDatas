## Description

<div><p>«Next please», — the princess called and cast an estimating glance at the next groom.</p><p>The princess intends to choose the most worthy groom, this is, the richest one. Whenever she sees a groom who is more rich than each of the previous ones, she says a measured «Oh...». Whenever the groom is richer than all previous ones added together, she exclaims «Wow!» (no «Oh...» in this case). At the sight of the first groom the princess stays calm and says nothing.</p><p>The fortune of each groom is described with an integer between 1 and 50000. You know that during the day the princess saw <span class="tex-span"><i>n</i></span> grooms, said «Oh...» exactly <span class="tex-span"><i>a</i></span> times and exclaimed «Wow!» exactly <span class="tex-span"><i>b</i></span> times. Your task is to output a sequence of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> describes the fortune of <span class="tex-span"><i>i</i></span>-th groom. If several sequences are possible, output any of them. If no sequence exists that would satisfy all the requirements, output a single number <span class="tex-font-style-tt">-1</span>.</p></div><div class="input-specification"><p>The only line of input data contains three integer numbers <span class="tex-span"><i>n</i>, <i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100, 0 ≤ <i>a</i>, <i>b</i> ≤ 15, <i>n</i> &gt; <i>a</i> + <i>b</i></span>), separated with single spaces.</p></div><div class="output-specification"><p>Output any sequence of integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 50000</span>) is the fortune of <span class="tex-span"><i>i</i></span>-th groom, that satisfies the given constraints. If no sequence exists that would satisfy all the requirements, output a single number <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The only line of input data contains three integer numbers <span class="tex-span"><i>n</i>, <i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100, 0 ≤ <i>a</i>, <i>b</i> ≤ 15, <i>n</i> &gt; <i>a</i> + <i>b</i></span>), separated with single spaces.</p>

## Output

<p>Output any sequence of integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 50000</span>) is the fortune of <span class="tex-span"><i>i</i></span>-th groom, that satisfies the given constraints. If no sequence exists that would satisfy all the requirements, output a single number <span class="tex-font-style-tt">-1</span>.</p>





```input1
10 2 3

```




```input2
5 0 0

```




```output1
5 1 3 6 16 35 46 4 200 99
```




```output2
10 10 6 6 5
```



## Note

<p>Let's have a closer look at the answer for the first sample test. </p><ul> <li> The princess said «Oh...» (highlighted in bold): 5 1 3 <span class="tex-font-style-bf">6</span> 16 35 <span class="tex-font-style-bf">46</span> 4 200 99. </li><li> The princess exclaimed «Wow!» (highlighted in bold): 5 1 3 6 <span class="tex-font-style-bf">16</span> <span class="tex-font-style-bf">35</span> 46 4 <span class="tex-font-style-bf">200</span> 99. </li></ul>
