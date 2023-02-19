## Description

<div><p>Little Timofey likes integers a lot. Unfortunately, he is very young and can't work with very big integers, so he does all the operations modulo his favorite prime <span class="tex-span"><i>m</i></span>. Also, Timofey likes to look for arithmetical progressions everywhere.</p><p>One of his birthday presents was a sequence of <span class="tex-font-style-bf">distinct</span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. Timofey wants to know whether he can rearrange the elements of the sequence so that is will be an arithmetical progression modulo <span class="tex-span"><i>m</i></span>, or not.</p><p>Arithmetical progression modulo <span class="tex-span"><i>m</i></span> of length <span class="tex-span"><i>n</i></span> with first element <span class="tex-span"><i>x</i></span> and difference <span class="tex-span"><i>d</i></span> is sequence of integers <span class="tex-span"><i>x</i>, <i>x</i> + <i>d</i>, <i>x</i> + 2<i>d</i>, ..., <i>x</i> + (<i>n</i> - 1)·<i>d</i></span>, each taken modulo <span class="tex-span"><i>m</i></span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup> + 7</span>, <span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span"><i>m</i></span> is prime)&nbsp;— Timofey's favorite prime module and the length of the sequence.</p><p>The second line contains <span class="tex-span"><i>n</i></span> <span class="tex-font-style-bf">distinct</span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>m</i></span>)&nbsp;— the elements of the sequence.</p></div><div class="output-specification"><p>Print <span class="tex-font-style-tt">-1</span> if it is not possible to rearrange the elements of the sequence so that is will be an arithmetical progression modulo <span class="tex-span"><i>m</i></span>.</p><p>Otherwise, print two integers&nbsp;— the first element of the obtained progression <span class="tex-span"><i>x</i></span> (<span class="tex-span">0 ≤ <i>x</i> &lt; <i>m</i></span>) and its difference <span class="tex-span"><i>d</i></span> (<span class="tex-span">0 ≤ <i>d</i> &lt; <i>m</i></span>).</p><p>If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup> + 7</span>, <span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span"><i>m</i></span> is prime)&nbsp;— Timofey's favorite prime module and the length of the sequence.</p><p>The second line contains <span class="tex-span"><i>n</i></span> <span class="tex-font-style-bf">distinct</span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>m</i></span>)&nbsp;— the elements of the sequence.</p>

## Output

<p>Print <span class="tex-font-style-tt">-1</span> if it is not possible to rearrange the elements of the sequence so that is will be an arithmetical progression modulo <span class="tex-span"><i>m</i></span>.</p><p>Otherwise, print two integers&nbsp;— the first element of the obtained progression <span class="tex-span"><i>x</i></span> (<span class="tex-span">0 ≤ <i>x</i> &lt; <i>m</i></span>) and its difference <span class="tex-span"><i>d</i></span> (<span class="tex-span">0 ≤ <i>d</i> &lt; <i>m</i></span>).</p><p>If there are multiple answers, print any of them.</p>





```input1
17 5
0 2 4 13 15

```




```input2
17 5
0 2 4 13 14

```




```input3
5 3
1 2 3

```




```output1
13 2

```




```output2
-1

```




```output3
3 4

```


