## Description

<div><p><span class="tex-font-style-it">We've got no test cases. A big olympiad is coming up. But the problemsetters' number one priority should be adding another problem to the round.</span> </p><p>The <span class="tex-font-style-bf">diameter</span> of a multiset of points on the line is the largest distance between two points from this set. For example, the diameter of the multiset <span class="tex-span">{1, 3, 2, 1}</span> is 2.</p><p>Diameter of multiset consisting of one point is 0.</p><p>You are given <span class="tex-span"><i>n</i></span> points on the line. What is the minimum number of points you have to remove, so that the diameter of the multiset of the remaining points will not exceed <span class="tex-span"><i>d</i></span>?</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100, 0 ≤ <i>d</i> ≤ 100</span>)&nbsp;— the amount of points and the maximum allowed diameter respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space separated integers (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>)&nbsp;— the coordinates of the points.</p></div><div class="output-specification"><p>Output a single integer&nbsp;— the minimum number of points you have to remove.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100, 0 ≤ <i>d</i> ≤ 100</span>)&nbsp;— the amount of points and the maximum allowed diameter respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space separated integers (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>)&nbsp;— the coordinates of the points.</p>

## Output

<p>Output a single integer&nbsp;— the minimum number of points you have to remove.</p>





```input1
3 1
2 1 4

```




```input2
3 0
7 7 7

```




```input3
6 3
1 3 4 6 9 10

```




```output1
1

```




```output2
0

```




```output3
3

```



## Note

<p>In the first test case the optimal strategy is to remove the point with coordinate <span class="tex-span">4</span>. The remaining points will have coordinates <span class="tex-span">1</span> and <span class="tex-span">2</span>, so the diameter will be equal to <span class="tex-span">2 - 1 = 1</span>.</p><p>In the second test case the diameter is equal to <span class="tex-span">0</span>, so its is unnecessary to remove any points. </p><p>In the third test case the optimal strategy is to remove points with coordinates <span class="tex-span">1</span>, <span class="tex-span">9</span> and <span class="tex-span">10</span>. The remaining points will have coordinates <span class="tex-span">3</span>, <span class="tex-span">4</span> and <span class="tex-span">6</span>, so the diameter will be equal to <span class="tex-span">6 - 3 = 3</span>.</p>
