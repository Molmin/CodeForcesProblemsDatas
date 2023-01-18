## Description

<div><p>Vasya has found a piece of paper with an array written on it. The array consists of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. Vasya noticed that the following condition holds for the array <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>a</i><sub class="lower-index"><i>i</i> + 1</sub> ≤ 2·<i>a</i><sub class="lower-index"><i>i</i></sub></span> for any positive integer <span class="tex-span"><i>i</i></span> (<span class="tex-span"><i>i</i> &lt; <i>n</i></span>).</p><p>Vasya wants to add either a "<span class="tex-font-style-tt">+</span>" or a "<span class="tex-font-style-tt">-</span>" before each number of array. Thus, Vasya will get an expression consisting of <span class="tex-span"><i>n</i></span> summands. The value of the resulting expression is the sum of all its elements. The task is to add signs "<span class="tex-font-style-tt">+</span>" and "<span class="tex-font-style-tt">-</span>" before each number so that the value of expression <span class="tex-span"><i>s</i></span> meets the limits <span class="tex-span">0 ≤ <i>s</i> ≤ <i>a</i><sub class="lower-index">1</sub></span>. Print a sequence of signs "<span class="tex-font-style-tt">+</span>" and "<span class="tex-font-style-tt">-</span>", satisfying the given limits. It is guaranteed that the solution for the problem exists.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the size of the array. The second line contains space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the original array. </p><p>It is guaranteed that the condition <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>a</i><sub class="lower-index"><i>i</i> + 1</sub> ≤ 2·<i>a</i><sub class="lower-index"><i>i</i></sub></span> fulfills for any positive integer <span class="tex-span"><i>i</i></span> (<span class="tex-span"><i>i</i> &lt; <i>n</i></span>).</p></div><div class="output-specification"><p>In a single line print the sequence of <span class="tex-span"><i>n</i></span> characters "<span class="tex-font-style-tt">+</span>" and "<span class="tex-font-style-tt">-</span>", where the <span class="tex-span"><i>i</i></span>-th character is the sign that is placed in front of number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. The value of the resulting expression <span class="tex-span"><i>s</i></span> must fit into the limits <span class="tex-span">0 ≤ <i>s</i> ≤ <i>a</i><sub class="lower-index">1</sub></span>. If there are multiple solutions, you are allowed to print any of them.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the size of the array. The second line contains space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the original array. </p><p>It is guaranteed that the condition <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>a</i><sub class="lower-index"><i>i</i> + 1</sub> ≤ 2·<i>a</i><sub class="lower-index"><i>i</i></sub></span> fulfills for any positive integer <span class="tex-span"><i>i</i></span> (<span class="tex-span"><i>i</i> &lt; <i>n</i></span>).</p>

## Output

<p>In a single line print the sequence of <span class="tex-span"><i>n</i></span> characters "<span class="tex-font-style-tt">+</span>" and "<span class="tex-font-style-tt">-</span>", where the <span class="tex-span"><i>i</i></span>-th character is the sign that is placed in front of number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. The value of the resulting expression <span class="tex-span"><i>s</i></span> must fit into the limits <span class="tex-span">0 ≤ <i>s</i> ≤ <i>a</i><sub class="lower-index">1</sub></span>. If there are multiple solutions, you are allowed to print any of them.</p>





```input1
4
1 2 3 5

```




```input2
3
3 3 5

```




```output1
+++-
```




```output2
++-
```


