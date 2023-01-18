## Description

<div><p>It's election time in Berland. The favorites are of course parties of zublicanes and mumocrates. The election campaigns of both parties include numerous demonstrations on <span class="tex-span"><i>n</i></span> main squares of the capital of Berland. Each of the <span class="tex-span"><i>n</i></span> squares certainly can have demonstrations of only one party, otherwise it could lead to riots. On the other hand, both parties have applied to host a huge number of demonstrations, so that on all squares demonstrations must be held. Now the capital management will distribute the area between the two parties.</p><p>Some pairs of squares are connected by <span class="tex-span">(<i>n</i> - 1)</span> bidirectional roads such that between any pair of squares there is a unique way to get from one square to another. Some squares are on the outskirts of the capital meaning that they are connected by a road with only one other square, such squares are called <span class="tex-font-style-it">dead end</span> squares.</p><p>The mayor of the capital instructed to distribute all the squares between the parties so that the <span class="tex-font-style-it">dead end</span> squares had the same number of demonstrations of the first and the second party. It is guaranteed that the number of dead end squares of the city is even.</p><p>To prevent possible conflicts between the zublicanes and the mumocrates it was decided to minimize the number of roads connecting the squares with the distinct parties. You, as a developer of the department of distributing squares, should determine this smallest number.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 5000</span>) — the number of squares in the capital of Berland.</p><p>Next <span class="tex-span"><i>n</i> - 1</span> lines contain the pairs of integers <span class="tex-span"><i>x</i>, <i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i>, <i>x</i> ≠ <i>y</i></span>) — the numbers of the squares connected by the road. All squares are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. It is guaranteed that the number of dead end squares of the city is even.</p></div><div class="output-specification"><p>Print a single number — the minimum number of roads connecting the squares with demonstrations of different parties.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 5000</span>) — the number of squares in the capital of Berland.</p><p>Next <span class="tex-span"><i>n</i> - 1</span> lines contain the pairs of integers <span class="tex-span"><i>x</i>, <i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i>, <i>x</i> ≠ <i>y</i></span>) — the numbers of the squares connected by the road. All squares are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. It is guaranteed that the number of dead end squares of the city is even.</p>

## Output

<p>Print a single number — the minimum number of roads connecting the squares with demonstrations of different parties.</p>





```input1
8
1 4
2 4
3 4
6 5
7 5
8 5
4 5

```




```input2
5
1 2
1 3
1 4
1 5

```




```output1
1

```




```output2
2

```


