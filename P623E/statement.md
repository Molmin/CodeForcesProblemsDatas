## Description

<div><p>Let's define the transformation <span class="tex-span"><i>P</i></span> of a sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> as <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> = <i>a</i><sub class="lower-index">1</sub>&nbsp;|&nbsp;<i>a</i><sub class="lower-index">2</sub>&nbsp;|&nbsp;...&nbsp;|&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub></span> for all <span class="tex-span"><i>i</i> = 1, 2, ..., <i>n</i></span>, where <span class="tex-span">|</span> is the bitwise OR operation.</p><p>Vasya consequently applies the transformation <span class="tex-span"><i>P</i></span> to all sequences of length <span class="tex-span"><i>n</i></span> consisting of integers from <span class="tex-span">1</span> to <span class="tex-span">2<sup class="upper-index"><i>k</i></sup> - 1</span> inclusive. He wants to know how many of these sequences have such property that their transformation is a <span class="tex-font-style-bf">strictly increasing</span> sequence. Help him to calculate this number modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The only line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup>, 1 ≤ <i>k</i> ≤ 30 000</span>).</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the answer to the problem modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The only line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup>, 1 ≤ <i>k</i> ≤ 30 000</span>).</p>

## Output

<p>Print a single integer&nbsp;— the answer to the problem modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
1 2

```




```input2
2 3

```




```input3
3 3

```




```output1
3

```




```output2
30

```




```output3
48

```


