## Description

<div><p>The Little Elephant is playing with the Cartesian coordinates' system. Most of all he likes playing with integer points. The Little Elephant defines an integer point as a pair of integers <span class="tex-span">(<i>x</i>;&nbsp;<i>y</i>)</span>, such that <span class="tex-span">0 ≤ <i>x</i> ≤ <i>w</i></span> and <span class="tex-span">0 ≤ <i>y</i> ≤ <i>h</i></span>. Thus, the Little Elephant knows only <span class="tex-span">(<i>w</i> + 1)·(<i>h</i> + 1)</span> distinct integer points.</p><p>The Little Elephant wants to paint a triangle with vertexes at integer points, the triangle's area must be a positive integer. For that, he needs to find the number of groups of three points that form such triangle. At that, the order of points in a group matters, that is, the group of three points <span class="tex-span">(0;0)</span>, <span class="tex-span">(0;2)</span>, <span class="tex-span">(2;2)</span> isn't equal to the group <span class="tex-span">(0;2)</span>, <span class="tex-span">(0;0)</span>, <span class="tex-span">(2;2)</span>.</p><p>Help the Little Elephant to find the number of groups of three integer points that form a nondegenerate triangle with integer area.</p></div><div class="input-specification"><p>A single line contains two integers <span class="tex-span"><i>w</i></span> and <span class="tex-span"><i>h</i></span> <span class="tex-span">(1 ≤ <i>w</i>, <i>h</i> ≤ 4000)</span>.</p></div><div class="output-specification"><p>In a single output line print an integer — the remainder of dividing the answer to the problem by <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>A single line contains two integers <span class="tex-span"><i>w</i></span> and <span class="tex-span"><i>h</i></span> <span class="tex-span">(1 ≤ <i>w</i>, <i>h</i> ≤ 4000)</span>.</p>

## Output

<p>In a single output line print an integer — the remainder of dividing the answer to the problem by <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
2 1

```




```input2
2 2

```




```output1
36

```




```output2
240

```


