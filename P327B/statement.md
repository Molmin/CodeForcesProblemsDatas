## Description

<div><p>Iahub and Iahubina went to a date at a luxury restaurant. Everything went fine until paying for the food. Instead of money, the waiter wants Iahub to write a Hungry sequence consisting of <span class="tex-span"><i>n</i></span> integers. </p><p>A sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span>, consisting of <span class="tex-span"><i>n</i></span> integers, is <span class="tex-font-style-it">Hungry</span> if and only if: </p><ul> <li> Its elements are in increasing order. That is an inequality <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>a</i><sub class="lower-index"><i>j</i></sub></span> holds for any two indices <span class="tex-span"><i>i</i>, <i>j</i></span> <span class="tex-span">(<i>i</i> &lt; <i>j</i>)</span>. </li><li> For any two indices <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> <span class="tex-span">(<i>i</i> &lt; <i>j</i>)</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> must <span class="tex-font-style-bf">not</span> be divisible by <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. </li></ul><p>Iahub is in trouble, so he asks you for help. Find a Hungry sequence with <span class="tex-span"><i>n</i></span> elements.</p></div><div class="input-specification"><p>The input contains a single integer: <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p></div><div class="output-specification"><p>Output a line that contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup>)</span>, representing a possible Hungry sequence. Note, that each <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> must not be greater than <span class="tex-span">10000000</span> (<span class="tex-span">10<sup class="upper-index">7</sup></span>) and less than <span class="tex-span">1</span>.</p><p>If there are multiple solutions you can output any one.</p></div>

## Input

<p>The input contains a single integer: <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p>

## Output

<p>Output a line that contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup>)</span>, representing a possible Hungry sequence. Note, that each <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> must not be greater than <span class="tex-span">10000000</span> (<span class="tex-span">10<sup class="upper-index">7</sup></span>) and less than <span class="tex-span">1</span>.</p><p>If there are multiple solutions you can output any one.</p>





```input1
3

```




```input2
5

```




```output1
2 9 15

```




```output2
11 14 20 27 31

```


