## Description

<div><p>A guy named Vasya attends the final grade of a high school. One day Vasya decided to watch a match of his favorite hockey team. And, as the boy loves hockey very much, even more than physics, he forgot to do the homework. Specifically, he forgot to complete his physics tasks. Next day the teacher got very angry at Vasya and decided to teach him a lesson. He gave the lazy student a seemingly easy task: You are given an idle body in space and the forces that affect it. The body can be considered as a material point with coordinates (0; 0; 0). Vasya had only to answer whether it is in equilibrium. "Piece of cake" — thought Vasya, we need only to check if the sum of all vectors is equal to 0. So, Vasya began to solve the problem. But later it turned out that there can be lots and lots of these forces, and Vasya can not cope without your help. Help him. Write a program that determines whether a body is idle or is moving by the given vectors of forces.</p></div><div class="input-specification"><p>The first line contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>), then follow <span class="tex-span"><i>n</i></span> lines containing three integers each: the <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> coordinate, the <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> coordinate and the <span class="tex-span"><i>z</i><sub class="lower-index"><i>i</i></sub></span> coordinate of the force vector, applied to the body (<span class="tex-span"> - 100 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>, <i>z</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>).</p></div><div class="output-specification"><p>Print the word "<span class="tex-font-style-tt">YES</span>" if the body is in equilibrium, or the word "<span class="tex-font-style-tt">NO</span>" if it is not.</p></div>

## Input

<p>The first line contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>), then follow <span class="tex-span"><i>n</i></span> lines containing three integers each: the <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> coordinate, the <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> coordinate and the <span class="tex-span"><i>z</i><sub class="lower-index"><i>i</i></sub></span> coordinate of the force vector, applied to the body (<span class="tex-span"> - 100 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>, <i>z</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>).</p>

## Output

<p>Print the word "<span class="tex-font-style-tt">YES</span>" if the body is in equilibrium, or the word "<span class="tex-font-style-tt">NO</span>" if it is not.</p>





```input1
3
4 1 7
-2 4 -1
1 -5 -3

```




```input2
3
3 -1 7
-5 2 -4
2 -1 -3

```




```output1
NO
```




```output2
YES
```


