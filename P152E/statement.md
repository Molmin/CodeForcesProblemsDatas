## Description

<div><p>Vasya has a very beautiful country garden that can be represented as an <span class="tex-span"><i>n</i> × <i>m</i></span> rectangular field divided into <span class="tex-span"><i>n</i>·<i>m</i></span> squares. One beautiful day Vasya remembered that he needs to pave roads between <span class="tex-span"><i>k</i></span> important squares that contain buildings. To pave a road, he can cover some squares of his garden with concrete.</p><p>For each garden square we know number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub><sub class="lower-index"><i>j</i></sub></span> that represents the number of flowers that grow in the square with coordinates <span class="tex-span">(<i>i</i>, <i>j</i>)</span>. When a square is covered with concrete, all flowers that grow in the square die.</p><p>Vasya wants to cover some squares with concrete so that the following conditions were fulfilled: </p><ul> <li> all <span class="tex-span"><i>k</i></span> important squares should necessarily be covered with concrete </li><li> from each important square there should be a way to any other important square. The way should go be paved with concrete-covered squares considering that neighboring squares are squares that have a common side </li><li> the total number of dead plants should be minimum </li></ul><p>As Vasya has a rather large garden, he asks you to help him.</p></div><div class="input-specification"><p>The first input line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>, <span class="tex-span"><i>n</i>·<i>m</i> ≤ 200</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>min</i>(<i>n</i>·<i>m</i>, 7</span>)) — the garden's sizes and the number of the important squares. Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub><sub class="lower-index"><i>j</i></sub> ≤ 1000</span>) — the numbers of flowers in the squares. Next <span class="tex-span"><i>k</i></span> lines contain coordinates of important squares written as "<span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span>" (without quotes) (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>y</i> ≤ <i>m</i></span>). The numbers written on one line are separated by spaces. It is guaranteed that all <span class="tex-span"><i>k</i></span> important squares have different coordinates.</p></div><div class="output-specification"><p>In the first line print the single integer — the minimum number of plants that die during the road construction. Then print <span class="tex-span"><i>n</i></span> lines each containing <span class="tex-span"><i>m</i></span> characters — the garden's plan. In this plan use character "<span class="tex-font-style-tt">X</span>" (uppercase Latin letter X) to represent a concrete-covered square and use character "." (dot) for a square that isn't covered with concrete. If there are multiple solutions, print any of them.</p></div>

## Input

<p>The first input line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>, <span class="tex-span"><i>n</i>·<i>m</i> ≤ 200</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>min</i>(<i>n</i>·<i>m</i>, 7</span>)) — the garden's sizes and the number of the important squares. Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub><sub class="lower-index"><i>j</i></sub> ≤ 1000</span>) — the numbers of flowers in the squares. Next <span class="tex-span"><i>k</i></span> lines contain coordinates of important squares written as "<span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span>" (without quotes) (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>y</i> ≤ <i>m</i></span>). The numbers written on one line are separated by spaces. It is guaranteed that all <span class="tex-span"><i>k</i></span> important squares have different coordinates.</p>

## Output

<p>In the first line print the single integer — the minimum number of plants that die during the road construction. Then print <span class="tex-span"><i>n</i></span> lines each containing <span class="tex-span"><i>m</i></span> characters — the garden's plan. In this plan use character "<span class="tex-font-style-tt">X</span>" (uppercase Latin letter X) to represent a concrete-covered square and use character "." (dot) for a square that isn't covered with concrete. If there are multiple solutions, print any of them.</p>





```input1
3 3 2
1 2 3
1 2 3
1 2 3
1 2
3 3

```




```input2
4 5 4
1 4 5 1 2
2 2 2 2 7
2 4 1 4 5
3 2 1 7 1
1 1
1 5
4 1
4 4

```




```output1
9
.X.
.X.
.XX

```




```output2
26
X..XX
XXXX.
X.X..
X.XX.

```


