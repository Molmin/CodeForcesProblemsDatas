## Description

<div><p>It's a very unfortunate day for Volodya today. He got bad mark in algebra and was therefore forced to do some work in the kitchen, namely to cook borscht (traditional Russian soup). This should also improve his algebra skills.</p><p>According to the borscht recipe it consists of <span class="tex-span"><i>n</i></span> ingredients that have to be mixed in proportion <img align="middle" class="tex-formula" src="file://PQ3LJP1M.png" style="max-width: 100.0%;max-height: 100.0%;"> litres (thus, there should be <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> ·<i>x</i>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub> ·<i>x</i></span> litres of corresponding ingredients mixed for some non-negative <span class="tex-span"><i>x</i></span>). In the kitchen Volodya found out that he has <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> litres of these ingredients at his disposal correspondingly. In order to correct his algebra mistakes he ought to cook as much soup as possible in a <span class="tex-span"><i>V</i></span> litres volume pan (which means the amount of soup cooked can be between <span class="tex-span">0</span> and <span class="tex-span"><i>V</i></span> litres). What is the volume of borscht Volodya will cook ultimately?</p></div><div class="input-specification"><p>The first line of the input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>V</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 20, 1 ≤ <i>V</i> ≤ 10000</span>). The next line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>). Finally, the last line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>).</p></div><div class="output-specification"><p>Your program should output just one real number — the volume of soup that Volodya will cook. Your answer must have a relative or absolute error less than <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p></div>

## Input

<p>The first line of the input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>V</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 20, 1 ≤ <i>V</i> ≤ 10000</span>). The next line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>). Finally, the last line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>).</p>

## Output

<p>Your program should output just one real number — the volume of soup that Volodya will cook. Your answer must have a relative or absolute error less than <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p>





```input1
1 100
1
40

```




```input2
2 100
1 1
25 30

```




```input3
2 100
1 1
60 60

```




```output1
40.0

```




```output2
50.0

```




```output3
100.0

```


