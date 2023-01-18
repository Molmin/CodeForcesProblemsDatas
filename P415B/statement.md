## Description

<div><p>Bimokh is Mashmokh's boss. For the following <span class="tex-span"><i>n</i></span> days he decided to pay to his workers in a new way. At the beginning of each day he will give each worker a certain amount of tokens. Then at the end of each day each worker can give some of his tokens back to get a certain amount of money. The worker can save the rest of tokens but he can't use it in any other day to get more money. If a worker gives back <span class="tex-span"><i>w</i></span> tokens then he'll get <img align="middle" class="tex-formula" src="file://1ESHbKS4.png" style="max-width: 100.0%;max-height: 100.0%;"> dollars. </p><p>Mashmokh likes the tokens however he likes money more. That's why he wants to save as many tokens as possible so that the amount of money he gets is maximal possible each day. He has <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span>. Number <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> is the number of tokens given to each worker on the <span class="tex-span"><i>i</i></span>-th day. Help him calculate for each of <span class="tex-span"><i>n</i></span> days the number of tokens he can save.</p></div><div class="input-specification"><p>The first line of input contains three space-separated integers <span class="tex-span"><i>n</i>, <i>a</i>, <i>b</i>&nbsp;(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">9</sup>)</span>. The second line of input contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub>&nbsp;(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>n</i></span> space-separated integers. The <span class="tex-span"><i>i</i></span>-th of them is the number of tokens Mashmokh can save on the <span class="tex-span"><i>i</i></span>-th day.</p></div>

## Input

<p>The first line of input contains three space-separated integers <span class="tex-span"><i>n</i>, <i>a</i>, <i>b</i>&nbsp;(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">9</sup>)</span>. The second line of input contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub>&nbsp;(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p>

## Output

<p>Output <span class="tex-span"><i>n</i></span> space-separated integers. The <span class="tex-span"><i>i</i></span>-th of them is the number of tokens Mashmokh can save on the <span class="tex-span"><i>i</i></span>-th day.</p>





```input1
5 1 4
12 6 11 9 1

```




```input2
3 1 2
1 2 3

```




```input3
1 1 1
1

```




```output1
0 2 3 1 1
```




```output2
1 0 1
```




```output3
0
```


