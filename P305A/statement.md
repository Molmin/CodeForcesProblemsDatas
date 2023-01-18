## Description

<div><p>Unfortunately, Vasya can only sum pairs of integers (<span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>), such that for any decimal place at least one number has digit <span class="tex-span">0</span> in this place. For example, Vasya can sum numbers <span class="tex-span">505</span> and <span class="tex-span">50</span>, but he cannot sum <span class="tex-span">1</span> and <span class="tex-span">4</span>.</p><p>Vasya has a set of <span class="tex-span"><i>k</i></span> distinct non-negative integers <span class="tex-span"><i>d</i><sub class="lower-index">1</sub>, <i>d</i><sub class="lower-index">2</sub>, ..., <i>d</i><sub class="lower-index"><i>k</i></sub></span>.</p><p>Vasya wants to choose some integers from this set so that he could sum any two chosen numbers. What maximal number of integers can he choose in the required manner?</p></div><div class="input-specification"><p>The first input line contains integer <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ 100)</span> — the number of integers.</p><p>The second line contains <span class="tex-span"><i>k</i></span> distinct space-separated integers <span class="tex-span"><i>d</i><sub class="lower-index">1</sub>, <i>d</i><sub class="lower-index">2</sub>, ..., <i>d</i><sub class="lower-index"><i>k</i></sub></span> <span class="tex-span">(0 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span>.</p></div><div class="output-specification"><p>In the first line print a single integer <span class="tex-span"><i>n</i></span> the maximum number of the chosen integers. In the second line print <span class="tex-span"><i>n</i></span> distinct non-negative integers — the required integers.</p><p>If there are multiple solutions, print any of them. You can print the numbers in any order.</p></div>

## Input

<p>The first input line contains integer <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ 100)</span> — the number of integers.</p><p>The second line contains <span class="tex-span"><i>k</i></span> distinct space-separated integers <span class="tex-span"><i>d</i><sub class="lower-index">1</sub>, <i>d</i><sub class="lower-index">2</sub>, ..., <i>d</i><sub class="lower-index"><i>k</i></sub></span> <span class="tex-span">(0 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span>.</p>

## Output

<p>In the first line print a single integer <span class="tex-span"><i>n</i></span> the maximum number of the chosen integers. In the second line print <span class="tex-span"><i>n</i></span> distinct non-negative integers — the required integers.</p><p>If there are multiple solutions, print any of them. You can print the numbers in any order.</p>





```input1
4
100 10 1 0

```




```input2
3
2 70 3

```




```output1
4
0 1 10 100
```




```output2
2
2 70
```


