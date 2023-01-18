## Description

<div><p>Vasya went for a walk in the park. The park has <span class="tex-span"><i>n</i></span> glades, numbered from 1 to <span class="tex-span"><i>n</i></span>. There are <span class="tex-span"><i>m</i></span> trails between the glades. The trails are numbered from 1 to <span class="tex-span"><i>m</i></span>, where the <span class="tex-span"><i>i</i></span>-th trail connects glades <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>. The numbers of the connected glades may be the same <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub> = <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>, which means that a trail connects a glade to itself. Also, two glades may have several non-intersecting trails between them.</p><p>Vasya is on glade 1, he wants to walk on all trails of the park exactly once, so that he can eventually return to glade 1. Unfortunately, Vasya does not know whether this walk is possible or not. Help Vasya, determine whether the walk is possible or not. If such walk is impossible, find the minimum number of trails the authorities need to add to the park in order to make the described walk possible.</p><p>Vasya can shift from one trail to another one only on glades. He can move on the trails in both directions. If Vasya started going on the trail that connects glades <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, from glade <span class="tex-span"><i>a</i></span>, then he must finish this trail on glade <span class="tex-span"><i>b</i></span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>;&nbsp;0 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup>)</span> — the number of glades in the park and the number of trails in the park, respectively. Next <span class="tex-span"><i>m</i></span> lines specify the trails. The <span class="tex-span"><i>i</i></span>-th line specifies the <span class="tex-span"><i>i</i></span>-th trail as two space-separated numbers, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the numbers of the glades connected by this trail.</p></div><div class="output-specification"><p>Print the single integer — the answer to the problem. If Vasya's walk is possible without adding extra trails, print <span class="tex-font-style-tt">0</span>, otherwise print the minimum number of trails the authorities need to add to the park in order to make Vasya's walk possible. </p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>;&nbsp;0 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup>)</span> — the number of glades in the park and the number of trails in the park, respectively. Next <span class="tex-span"><i>m</i></span> lines specify the trails. The <span class="tex-span"><i>i</i></span>-th line specifies the <span class="tex-span"><i>i</i></span>-th trail as two space-separated numbers, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the numbers of the glades connected by this trail.</p>

## Output

<p>Print the single integer — the answer to the problem. If Vasya's walk is possible without adding extra trails, print <span class="tex-font-style-tt">0</span>, otherwise print the minimum number of trails the authorities need to add to the park in order to make Vasya's walk possible. </p>





```input1
3 3
1 2
2 3
3 1

```




```input2
2 5
1 1
1 2
1 2
2 2
1 2

```




```output1
0

```




```output2
1

```



## Note

<p>In the first test case the described walk is possible without building extra trails. For example, let's first go on the first trail, then on the second one, and finally on the third one.</p><p>In the second test case the described walk is impossible without adding extra trails. To make the walk possible, it is enough to add one trail, for example, between glades number one and two.</p>
