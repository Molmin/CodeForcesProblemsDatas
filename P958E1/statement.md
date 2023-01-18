## Description

<div><p>The Rebel fleet is afraid that the Empire might want to strike back again. Princess Heidi needs to know if it is possible to assign <span class="tex-span"><i>R</i></span> Rebel spaceships to guard <span class="tex-span"><i>B</i></span> bases so that every base has exactly one guardian and each spaceship has exactly one assigned base (in other words, the assignment is a perfect matching). Since she knows how reckless her pilots are, she wants to be sure that any two (straight) paths – from a base to its assigned spaceship – do not intersect in the galaxy plane (that is, in 2D), and so there is no risk of collision.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>R</i>, <i>B</i>(1 ≤ <i>R</i>, <i>B</i> ≤ 10)</span>. For <span class="tex-span">1 ≤ <i>i</i> ≤ <i>R</i></span>, the <span class="tex-span"><i>i</i> + 1</span>-th line contains two space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10000</span>) denoting the coordinates of the <span class="tex-span"><i>i</i></span>-th Rebel spaceship. The following <span class="tex-span"><i>B</i></span> lines have the same format, denoting the position of bases. It is guaranteed that no two points coincide and that no three points are on the same line.</p></div><div class="output-specification"><p>If it is possible to connect Rebel spaceships and bases so as satisfy the constraint, output <span class="tex-font-style-tt">Yes</span>, otherwise output <span class="tex-font-style-tt">No</span> (without quote).</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>R</i>, <i>B</i>(1 ≤ <i>R</i>, <i>B</i> ≤ 10)</span>. For <span class="tex-span">1 ≤ <i>i</i> ≤ <i>R</i></span>, the <span class="tex-span"><i>i</i> + 1</span>-th line contains two space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10000</span>) denoting the coordinates of the <span class="tex-span"><i>i</i></span>-th Rebel spaceship. The following <span class="tex-span"><i>B</i></span> lines have the same format, denoting the position of bases. It is guaranteed that no two points coincide and that no three points are on the same line.</p>

## Output

<p>If it is possible to connect Rebel spaceships and bases so as satisfy the constraint, output <span class="tex-font-style-tt">Yes</span>, otherwise output <span class="tex-font-style-tt">No</span> (without quote).</p>





```input1
3 3
0 0
2 0
3 1
-2 1
0 3
2 2

```




```input2
2 1
1 0
2 2
3 1

```




```output1
Yes

```




```output2
No

```



## Note

<p>For the first example, one possible way is to connect the Rebels and bases in order.</p><p>For the second example, there is no perfect matching between Rebels and bases.</p>
