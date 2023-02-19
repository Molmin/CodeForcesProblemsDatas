## Description

<div><p>Pavel cooks barbecue. There are <span class="tex-span"><i>n</i></span> skewers, they lay on a brazier in a row, each on one of <span class="tex-span"><i>n</i></span> positions. Pavel wants each skewer to be cooked some time in every of <span class="tex-span"><i>n</i></span> positions in two directions: in the one it was directed originally and in the reversed direction.</p><p>Pavel has a plan: a permutation <span class="tex-span"><i>p</i></span> and a sequence <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span>, consisting of zeros and ones. Each second Pavel move skewer on position <span class="tex-span"><i>i</i></span> to position <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, and if <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> equals <span class="tex-span">1</span> then he reverses it. So he hope that every skewer will visit every position in both directions.</p><p>Unfortunately, not every pair of permutation <span class="tex-span"><i>p</i></span> and sequence <span class="tex-span"><i>b</i></span> suits Pavel. What is the minimum total number of elements in the given permutation <span class="tex-span"><i>p</i></span> and the given sequence <span class="tex-span"><i>b</i></span> he needs to change so that every skewer will visit each of <span class="tex-span">2<i>n</i></span> placements? Note that after changing the permutation should remain a permutation as well.</p><p>There is no problem for Pavel, if some skewer visits some of the placements several times before he ends to cook. In other words, a permutation <span class="tex-span"><i>p</i></span> and a sequence <span class="tex-span"><i>b</i></span> suit him if there is an integer <span class="tex-span"><i>k</i></span> (<span class="tex-span"><i>k</i> ≥ 2<i>n</i></span>), so that after <span class="tex-span"><i>k</i></span> seconds each skewer visits each of the <span class="tex-span">2<i>n</i></span> placements.</p><p>It can be shown that some suitable pair of permutation <span class="tex-span"><i>p</i></span> and sequence <span class="tex-span"><i>b</i></span> exists for any <span class="tex-span"><i>n</i></span>.</p></div><div class="input-specification"><p>The first line contain the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of skewers.</p><p>The second line contains a sequence of integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the permutation, according to which Pavel wants to move the skewers.</p><p>The third line contains a sequence <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> consisting of zeros and ones, according to which Pavel wants to reverse the skewers.</p></div><div class="output-specification"><p>Print single integer&nbsp;— the minimum total number of elements in the given permutation <span class="tex-span"><i>p</i></span> and the given sequence <span class="tex-span"><i>b</i></span> he needs to change so that every skewer will visit each of <span class="tex-span">2<i>n</i></span> placements.</p></div>

## Input

<p>The first line contain the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of skewers.</p><p>The second line contains a sequence of integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the permutation, according to which Pavel wants to move the skewers.</p><p>The third line contains a sequence <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> consisting of zeros and ones, according to which Pavel wants to reverse the skewers.</p>

## Output

<p>Print single integer&nbsp;— the minimum total number of elements in the given permutation <span class="tex-span"><i>p</i></span> and the given sequence <span class="tex-span"><i>b</i></span> he needs to change so that every skewer will visit each of <span class="tex-span">2<i>n</i></span> placements.</p>





```input1
4
4 3 2 1
0 1 1 1

```




```input2
3
2 3 1
0 0 0

```




```output1
2

```




```output2
1

```



## Note

<p>In the first example Pavel can change the permutation to <span class="tex-span">4, 3, 1, 2</span>.</p><p>In the second example Pavel can change any element of <span class="tex-span"><i>b</i></span> to <span class="tex-span">1</span>.</p>
