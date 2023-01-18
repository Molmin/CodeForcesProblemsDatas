## Description

<div><p>In this task Anna and Maria play the following game. Initially they have a checkered piece of paper with a painted <span class="tex-span"><i>n</i> × <i>m</i></span> rectangle (only the border, no filling). Anna and Maria move in turns and Anna starts. During each move one should paint inside the last-painted rectangle a new lesser rectangle (along the grid lines). The new rectangle should have no common points with the previous one. Note that when we paint a rectangle, we always paint only the border, the rectangles aren't filled.</p><p>Nobody wins the game — Anna and Maria simply play until they have done <span class="tex-span"><i>k</i></span> moves in total. Count the number of different ways to play this game.</p></div><div class="input-specification"><p>The first and only line contains three integers: <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>k</i> ≤ 1000</span>).</p></div><div class="output-specification"><p>Print the single number — the number of the ways to play the game. As this number can be very big, print the value modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div>

## Input

<p>The first and only line contains three integers: <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>k</i> ≤ 1000</span>).</p>

## Output

<p>Print the single number — the number of the ways to play the game. As this number can be very big, print the value modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p>





```input1
3 3 1

```




```input2
4 4 1

```




```input3
6 7 2

```




```output1
1

```




```output2
9

```




```output3
75

```



## Note

<p>Two ways to play the game are considered different if the final pictures are different. In other words, if one way contains a rectangle that is not contained in the other way.</p><p>In the first sample Anna, who performs her first and only move, has only one possible action plan — insert a <span class="tex-span">1 × 1</span> square inside the given <span class="tex-span">3 × 3</span> square.</p><p>In the second sample Anna has as much as 9 variants: 4 ways to paint a <span class="tex-span">1 × 1</span> square, 2 ways to insert a <span class="tex-span">1 × 2</span> rectangle vertically, 2 more ways to insert it horizontally and one more way is to insert a <span class="tex-span">2 × 2</span> square.</p>
