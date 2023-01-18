## Description

<div><p>You are given an array <span class="tex-span"><i>a</i></span> consisting of <span class="tex-span"><i>n</i></span> integers, and additionally an integer <span class="tex-span"><i>m</i></span>. You have to choose some sequence of indices <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index">1</sub> &lt; <i>b</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>b</i><sub class="lower-index"><i>k</i></sub> ≤ <i>n</i></span>) in such a way that the value of <img align="middle" class="tex-formula" src="file://8Uhvc6qp.png" style="max-width: 100.0%;max-height: 100.0%;"> is maximized. Chosen sequence can be empty.</p><p>Print the maximum possible value of <img align="middle" class="tex-formula" src="file://s5A2UaAT.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 35</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print the maximum possible value of <img align="middle" class="tex-formula" src="file://LcYu97cd.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 35</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print the maximum possible value of <img align="middle" class="tex-formula" src="file://LcYu97cd.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
4 4
5 2 4 1

```




```input2
3 20
199 41 299

```




```output1
3

```




```output2
19

```



## Note

<p>In the first example you can choose a sequence <span class="tex-span"><i>b</i> = {1, 2}</span>, so the sum <img align="middle" class="tex-formula" src="file://yyMvUJto.png" style="max-width: 100.0%;max-height: 100.0%;"> is equal to <span class="tex-span">7</span> (and that's <span class="tex-span">3</span> after taking it modulo <span class="tex-span">4</span>).</p><p>In the second example you can choose a sequence <span class="tex-span"><i>b</i> = {3}</span>.</p>
