## Description

<div><p>People in the Tomskaya region like magic formulas very much. You can see some of them below.</p><p>Imagine you are given a sequence of positive integer numbers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>p</i><sub class="lower-index"><i>n</i></sub></span>. Lets write down some magic formulas:</p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://8nJmTwYa.png" style="max-width: 100.0%;max-height: 100.0%;"></center><center class="tex-equation"><img align="middle" class="tex-formula" src="file://TTdVipyl.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>Here, "<span class="tex-font-style-tt">mod</span>" means the operation of taking the residue after dividing.</p><p>The expression <img align="middle" class="tex-formula" src="file://MBZIwB7S.png" style="max-width: 100.0%;max-height: 100.0%;"> means applying the bitwise <span class="tex-span"><i>xor</i></span> (excluding "OR") operation to integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>. The given operation exists in all modern programming languages. For example, in languages C++ and Java it is represented by "<span class="tex-font-style-tt">^</span>", in Pascal — by "xor".</p><p>People in the Tomskaya region like magic formulas very much, but they don't like to calculate them! Therefore you are given the sequence <span class="tex-span"><i>p</i></span>, calculate the value of <span class="tex-span"><i>Q</i></span>.</p></div><div class="input-specification"><p>The first line of the input contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>). The next line contains <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>The only line of output should contain a single integer — the value of <span class="tex-span"><i>Q</i></span>.</p></div>

## Input

<p>The first line of the input contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>). The next line contains <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>The only line of output should contain a single integer — the value of <span class="tex-span"><i>Q</i></span>.</p>





```input1
3
1 2 3

```




```output1
3

```


