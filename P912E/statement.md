## Description

<div><p>Opposite to Grisha's nice behavior, Oleg, though he has an entire year at his disposal, didn't manage to learn how to solve number theory problems in the past year. That's why instead of Ded Moroz he was visited by his teammate Andrew, who solemnly presented him with a set of <span class="tex-span"><i>n</i></span> <span class="tex-font-style-bf">distinct prime</span> numbers alongside with a simple task: Oleg is to find the <span class="tex-span"><i>k</i></span>-th smallest integer, such that <span class="tex-font-style-bf">all</span> its prime divisors are in this set. </p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 16</span>).</p><p>The next line lists <span class="tex-span"><i>n</i></span> distinct prime numbers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">2 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) in ascending order.</p><p>The last line gives a single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i></span>). It is guaranteed that the <span class="tex-span"><i>k</i></span>-th smallest integer such that all its prime divisors are in this set does not exceed <span class="tex-span">10<sup class="upper-index">18</sup></span>.</p></div><div class="output-specification"><p>Print a single line featuring the <span class="tex-span"><i>k</i></span>-th smallest integer. It's guaranteed that the answer doesn't exceed <span class="tex-span">10<sup class="upper-index">18</sup></span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 16</span>).</p><p>The next line lists <span class="tex-span"><i>n</i></span> distinct prime numbers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">2 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) in ascending order.</p><p>The last line gives a single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i></span>). It is guaranteed that the <span class="tex-span"><i>k</i></span>-th smallest integer such that all its prime divisors are in this set does not exceed <span class="tex-span">10<sup class="upper-index">18</sup></span>.</p>

## Output

<p>Print a single line featuring the <span class="tex-span"><i>k</i></span>-th smallest integer. It's guaranteed that the answer doesn't exceed <span class="tex-span">10<sup class="upper-index">18</sup></span>.</p>





```input1
3
2 3 5
7

```




```input2
5
3 7 11 13 31
17

```




```output1
8

```




```output2
93

```



## Note

<p>The list of numbers with all prime divisors inside <span class="tex-span">{2, 3, 5}</span> begins as follows:</p><p><span class="tex-span">(1, 2, 3, 4, 5, 6, 8, ...)</span></p><p>The seventh number in this list (<span class="tex-span">1</span>-indexed) is eight.</p>
