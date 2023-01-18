## Description

<div><p>Little boy Valera studies an algorithm of sorting an integer array. After studying the theory, he went on to the practical tasks. As a result, he wrote a program that sorts an array of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> in the non-decreasing order. The pseudocode of the program, written by Valera, is given below. The input of the program gets number <span class="tex-span"><i>n</i></span> and array <span class="tex-span"><i>a</i></span>.</p><pre class="verbatim"><br>loop integer variable <span class="tex-span"><i>i</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i> - 1</span><br>&nbsp;&nbsp;&nbsp;&nbsp;loop integer variable <span class="tex-span"><i>j</i></span> from <span class="tex-span"><i>i</i></span> to <span class="tex-span"><i>n</i> - 1</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;if <span class="tex-span">(<i>a</i><sub class="lower-index"><i>j</i></sub> &gt; <i>a</i><sub class="lower-index"><i>j</i> + 1</sub>)</span>, then swap the values of elements <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i> + 1</sub></span><br></pre><p>But Valera could have made a mistake, because he hasn't yet fully learned the sorting algorithm. If Valera made a mistake in his program, you need to give a counter-example that makes his program work improperly (that is, the example that makes the program sort the array not in the non-decreasing order). If such example for the given value of <span class="tex-span"><i>n</i></span> doesn't exist, print -1.</p></div><div class="input-specification"><p>You've got a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 50)</span> — the size of the sorted array.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the counter-example, for which Valera's algorithm won't work correctly. If the counter-example that meets the described conditions is impossible to give, print -1.</p><p>If there are several counter-examples, consisting of <span class="tex-span"><i>n</i></span> numbers, you are allowed to print any of them.</p></div>

## Input

<p>You've got a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 50)</span> — the size of the sorted array.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the counter-example, for which Valera's algorithm won't work correctly. If the counter-example that meets the described conditions is impossible to give, print -1.</p><p>If there are several counter-examples, consisting of <span class="tex-span"><i>n</i></span> numbers, you are allowed to print any of them.</p>





```input1
1

```




```output1
-1

```


