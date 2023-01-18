## Description

<div><p>Iahub is playing an uncommon game. Initially, he has <span class="tex-span"><i>n</i></span> boxes, numbered 1, 2, 3, <span class="tex-span">...</span>, <span class="tex-span"><i>n</i></span>. Each box has some number of candies in it, described by a sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span>. The number <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i></sub></span> represents the number of candies in box <span class="tex-span"><i>k</i></span>. </p><p>The goal of the game is to move all candies into <span class="tex-font-style-bf">exactly</span> two boxes. The rest of <span class="tex-span"><i>n</i> - 2</span> boxes must contain <span class="tex-font-style-bf">zero</span> candies. Iahub is allowed to do several (possible zero) moves. At each move he chooses two different boxes <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span>, such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>a</i><sub class="lower-index"><i>j</i></sub></span>. Then, Iahub moves from box <span class="tex-span"><i>j</i></span> to box <span class="tex-span"><i>i</i></span> exactly <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> candies. Obviously, when two boxes have equal number of candies, box number <span class="tex-span"><i>j</i></span> becomes empty.</p><p>Your task is to give him a set of moves such as Iahub to archive the goal of the game. If Iahub can't win the game for the given configuration of boxes, output -1. Please note that in case there exist a solution, you don't need to print the solution using minimal number of moves.</p></div><div class="input-specification"><p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 1000</span>). The next line contains <span class="tex-span"><i>n</i></span> non-negative integers: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> — sequence elements. It is guaranteed that sum of all numbers in sequence <span class="tex-span"><i>a</i></span> is up to <span class="tex-span">10<sup class="upper-index">6</sup></span>. </p></div><div class="output-specification"><p>In case there exists no solution, output -1. Otherwise, in the first line output integer <span class="tex-span"><i>c</i></span> <span class="tex-span">(0 ≤ <i>c</i> ≤ 10<sup class="upper-index">6</sup>)</span>, representing number of moves in your solution. Each of the next <span class="tex-span"><i>c</i></span> lines should contain two integers <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> <span class="tex-span">(1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i>, <i>i</i> ≠ <i>j</i>)</span>: integers <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>j</i></span> in the <span class="tex-span"><i>k</i></span>th line mean that at the <span class="tex-span"><i>k</i></span>-th move you will move candies from the <span class="tex-span"><i>j</i></span>-th box to the <span class="tex-span"><i>i</i></span>-th one.</p></div>

## Input

<p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 1000</span>). The next line contains <span class="tex-span"><i>n</i></span> non-negative integers: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> — sequence elements. It is guaranteed that sum of all numbers in sequence <span class="tex-span"><i>a</i></span> is up to <span class="tex-span">10<sup class="upper-index">6</sup></span>. </p>

## Output

<p>In case there exists no solution, output -1. Otherwise, in the first line output integer <span class="tex-span"><i>c</i></span> <span class="tex-span">(0 ≤ <i>c</i> ≤ 10<sup class="upper-index">6</sup>)</span>, representing number of moves in your solution. Each of the next <span class="tex-span"><i>c</i></span> lines should contain two integers <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> <span class="tex-span">(1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i>, <i>i</i> ≠ <i>j</i>)</span>: integers <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>j</i></span> in the <span class="tex-span"><i>k</i></span>th line mean that at the <span class="tex-span"><i>k</i></span>-th move you will move candies from the <span class="tex-span"><i>j</i></span>-th box to the <span class="tex-span"><i>i</i></span>-th one.</p>





```input1
3
3 6 9

```




```input2
3
0 1 0

```




```input3
4
0 1 1 0

```




```output1
2
2 3
1 3

```




```output2
-1
```




```output3
0

```



## Note

<p>For the first sample, after the first move the boxes will contain 3, 12 and 3 candies. After the second move, the boxes will contain 6, 12 and 0 candies. Now all candies are in exactly 2 boxes.</p><p>For the second sample, you can observe that the given configuration is not valid, as all candies are in a single box and they should be in two boxes. Also, any move won't change the configuration, so there exists no solution.</p><p>For the third sample, all candies are already in 2 boxes. Hence, no move is needed.</p>
