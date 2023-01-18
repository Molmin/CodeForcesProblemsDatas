## Description

<div><p><span class="tex-font-style-it">Mashmokh's boss, Bimokh, didn't like Mashmokh. So he fired him. Mashmokh decided to go to university and participate in ACM instead of finding a new job. He wants to become a member of Bamokh's team. In order to join he was given some programming tasks and one week to solve them. Mashmokh is not a very experienced programmer. Actually he is not a programmer at all. So he wasn't able to solve them. That's why he asked you to help him with these tasks. One of these tasks is the following.</span></p><p>A sequence of <span class="tex-span"><i>l</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>l</i></sub></span> <span class="tex-span">(1 ≤ <i>b</i><sub class="lower-index">1</sub> ≤ <i>b</i><sub class="lower-index">2</sub> ≤ ... ≤ <i>b</i><sub class="lower-index"><i>l</i></sub> ≤ <i>n</i>)</span> is called <span class="tex-font-style-it">good</span> if each number divides (without a remainder) by the next number in the sequence. More formally <img align="middle" class="tex-formula" src="file://Yd74V7oU.png" style="max-width: 100.0%;max-height: 100.0%;"> for all <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>l</i> - 1)</span>.</p><p>Given <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> find the number of good sequences of length <span class="tex-span"><i>k</i></span>. As the answer can be rather large print it modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div><div class="input-specification"><p>The first line of input contains two space-separated integers <span class="tex-span"><i>n</i>, <i>k</i>&nbsp;(1 ≤ <i>n</i>, <i>k</i> ≤ 2000)</span>.</p></div><div class="output-specification"><p>Output a single integer — the number of good sequences of length <span class="tex-span"><i>k</i></span> modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line of input contains two space-separated integers <span class="tex-span"><i>n</i>, <i>k</i>&nbsp;(1 ≤ <i>n</i>, <i>k</i> ≤ 2000)</span>.</p>

## Output

<p>Output a single integer — the number of good sequences of length <span class="tex-span"><i>k</i></span> modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
3 2

```




```input2
6 4

```




```input3
2 1

```




```output1
5

```




```output2
39

```




```output3
2

```



## Note

<p>In the first sample the good sequences are: <span class="tex-span">[1, 1], [2, 2], [3, 3], [1, 2], [1, 3]</span>.</p>
