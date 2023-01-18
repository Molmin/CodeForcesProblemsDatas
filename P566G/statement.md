## Description

<div><p>Two kittens, Max and Min, play with a pair of non-negative integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>. As you can guess from their names, kitten Max loves to maximize and kitten Min loves to minimize. As part of this game Min wants to make sure that both numbers, <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> became negative at the same time, and kitten Max tries to prevent him from doing so.</p><p>Each kitten has a set of pairs of integers available to it. Kitten Max has <span class="tex-span"><i>n</i></span> pairs of non-negative integers <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>), and kitten Min has <span class="tex-span"><i>m</i></span> pairs of non-negative integers <span class="tex-span">(<i>c</i><sub class="lower-index"><i>j</i></sub>, <i>d</i><sub class="lower-index"><i>j</i></sub>)</span> (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>m</i></span>). As kitten Max makes a move, it can take any available pair <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> and add <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>y</i></span>, and kitten Min can take any available pair <span class="tex-span">(<i>c</i><sub class="lower-index"><i>j</i></sub>, <i>d</i><sub class="lower-index"><i>j</i></sub>)</span> and subtract <span class="tex-span"><i>c</i><sub class="lower-index"><i>j</i></sub></span> from <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>d</i><sub class="lower-index"><i>j</i></sub></span> from <span class="tex-span"><i>y</i></span>. Each kitten can use each pair multiple times during distinct moves.</p><p>Max moves first. Kitten Min is winning if at some moment both numbers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> are negative <span class="tex-font-style-bf">simultaneously</span>. Otherwise, the winner of the game is kitten Max. Determine which kitten wins if both of them play optimally.</p></div><div class="input-specification"><p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100 000</span>) — the number of pairs of numbers available to Max and Min, correspondingly.</p><p>The second line contains two integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">9</sup></span>) — the initial values of numbers with which the kittens are playing.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain the pairs of numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the pairs available to Max.</p><p>The last <span class="tex-span"><i>m</i></span> lines contain pairs of numbers <span class="tex-span"><i>c</i><sub class="lower-index"><i>j</i></sub>, <i>d</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>j</i></sub>, <i>d</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the pairs available to Min.</p></div><div class="output-specification"><p>Print «<span class="tex-font-style-tt">Max</span>» (without the quotes), if kitten Max wins, or "<span class="tex-font-style-tt">Min</span>" (without the quotes), if kitten Min wins.</p></div>

## Input

<p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100 000</span>) — the number of pairs of numbers available to Max and Min, correspondingly.</p><p>The second line contains two integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">9</sup></span>) — the initial values of numbers with which the kittens are playing.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain the pairs of numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the pairs available to Max.</p><p>The last <span class="tex-span"><i>m</i></span> lines contain pairs of numbers <span class="tex-span"><i>c</i><sub class="lower-index"><i>j</i></sub>, <i>d</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>j</i></sub>, <i>d</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the pairs available to Min.</p>

## Output

<p>Print «<span class="tex-font-style-tt">Max</span>» (without the quotes), if kitten Max wins, or "<span class="tex-font-style-tt">Min</span>" (without the quotes), if kitten Min wins.</p>





```input1
2 2
42 43
2 3
3 2
3 10
10 3

```




```input2
1 1
1 1
3 4
1 1

```




```output1
Min

```




```output2
Max

```



## Note

<p>In the first test from the statement Min can respond to move <span class="tex-span">(2, 3)</span> by move <span class="tex-span">(3, 10)</span>, and to move <span class="tex-span">(3, 2)</span> by move <span class="tex-span">(10, 3)</span>. Thus, for each pair of Max and Min's moves the values of both numbers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> will strictly decrease, ergo, Min will win sooner or later.</p><p>In the second sample test after each pair of Max and Min's moves both numbers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> only increase, thus none of them will become negative.</p>
