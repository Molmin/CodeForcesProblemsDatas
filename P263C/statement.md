## Description

<div><p>One day Vasya came up to the blackboard and wrote out <span class="tex-span"><i>n</i></span> distinct integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in some order in a circle. Then he drew arcs to join the pairs of integers <span class="tex-span">(<i>a</i>, <i>b</i>)</span> <span class="tex-span">(<i>a</i> ≠ <i>b</i>)</span>, that are either each other's immediate neighbors in the circle, or there is number <span class="tex-span"><i>c</i></span>, such that <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>с</i></span> are immediate neighbors, and <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> are immediate neighbors. As you can easily deduce, in the end Vasya drew <span class="tex-span">2·<i>n</i></span> arcs.</p><p>For example, if the numbers are written in the circle in the order <span class="tex-span">1, 2, 3, 4, 5</span> (in the clockwise direction), then the arcs will join pairs of integers <span class="tex-span">(1, 2)</span>, <span class="tex-span">(2, 3)</span>, <span class="tex-span">(3, 4)</span>, <span class="tex-span">(4, 5)</span>, <span class="tex-span">(5, 1)</span>, <span class="tex-span">(1, 3)</span>, <span class="tex-span">(2, 4)</span>, <span class="tex-span">(3, 5)</span>, <span class="tex-span">(4, 1)</span> and <span class="tex-span">(5, 2)</span>.</p><p>Much time has passed ever since, the numbers we wiped off the blackboard long ago, but recently Vasya has found a piece of paper with <span class="tex-span">2·<i>n</i></span> written pairs of integers that were joined with the arcs on the board. Vasya asks you to find the order of numbers in the circle by these pairs.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">5 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) that shows, how many numbers were written on the board. Next <span class="tex-span">2·<i>n</i></span> lines contain pairs of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>) — the numbers that were connected by the arcs.</p><p>It is guaranteed that no pair of integers, connected by a arc, occurs in the input more than once. The pairs of numbers and the numbers in the pairs are given in the arbitrary order.</p></div><div class="output-specification"><p>If Vasya made a mistake somewhere and there isn't any way to place numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> on the circle according to the statement, then print a single number "-1" (without the quotes). Otherwise, print any suitable sequence of <span class="tex-span"><i>n</i></span> distinct integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. </p><p>If there are multiple solutions, you are allowed to print any of them. Specifically, it doesn't matter which number you write first to describe the sequence of the order. It also doesn't matter whether you write out the numbers in the clockwise or counter-clockwise direction.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">5 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) that shows, how many numbers were written on the board. Next <span class="tex-span">2·<i>n</i></span> lines contain pairs of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>) — the numbers that were connected by the arcs.</p><p>It is guaranteed that no pair of integers, connected by a arc, occurs in the input more than once. The pairs of numbers and the numbers in the pairs are given in the arbitrary order.</p>

## Output

<p>If Vasya made a mistake somewhere and there isn't any way to place numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> on the circle according to the statement, then print a single number "-1" (without the quotes). Otherwise, print any suitable sequence of <span class="tex-span"><i>n</i></span> distinct integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. </p><p>If there are multiple solutions, you are allowed to print any of them. Specifically, it doesn't matter which number you write first to describe the sequence of the order. It also doesn't matter whether you write out the numbers in the clockwise or counter-clockwise direction.</p>





```input1
5
1 2
2 3
3 4
4 5
5 1
1 3
2 4
3 5
4 1
5 2

```




```input2
6
5 6
4 3
5 3
2 4
6 1
3 1
6 2
2 5
1 4
3 6
1 2
4 5

```




```output1
1 2 3 4 5
```




```output2
1 2 4 5 3 6
```


