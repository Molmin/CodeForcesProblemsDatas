## Description

<div><p>Little Chris is very keen on his toy blocks. His teacher, however, wants Chris to solve more problems, so he decided to play a trick on Chris.</p><p>There are exactly <span class="tex-span"><i>s</i></span> blocks in Chris's set, each block has a unique number from 1 to <span class="tex-span"><i>s</i></span>. Chris's teacher picks a subset of blocks <span class="tex-span"><i>X</i></span> and keeps it to himself. He will give them back only if Chris can pick such a non-empty subset <span class="tex-span"><i>Y</i></span> from the remaining blocks, that the equality holds: </p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://c2wqtP8P.png" style="max-width: 100.0%;max-height: 100.0%;"></center> "Are you kidding me?", asks Chris.<p>For example, consider a case where <span class="tex-span"><i>s</i> = 8</span> and Chris's teacher took the blocks with numbers 1, 4 and 5. One way for Chris to choose a set is to pick the blocks with numbers 3 and 6, see figure. Then the required sums would be equal: <span class="tex-span">(1 - 1) + (4 - 1) + (5 - 1) = (8 - 3) + (8 - 6) = 7</span>.</p><center> <img class="tex-graphics" src="file://1hBow2R5.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>However, now Chris has exactly <span class="tex-span"><i>s</i> = 10<sup class="upper-index">6</sup></span> blocks. Given the set <span class="tex-span"><i>X</i></span> of blocks his teacher chooses, help Chris to find the required set <span class="tex-span"><i>Y</i></span>!</p></div><div class="input-specification"><p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>), the number of blocks in the set <span class="tex-span"><i>X</i></span>. The next line contains <span class="tex-span"><i>n</i></span> distinct space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>), the numbers of the blocks in <span class="tex-span"><i>X</i></span>.</p><p><span class="tex-font-style-bf">Note</span>: since the size of the input and output could be very large, don't use slow output techniques in your language. For example, do not use input and output streams (cin, cout) in C++.</p></div><div class="output-specification"><p>In the first line of output print a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup> - <i>n</i></span>), the number of blocks in the set <span class="tex-span"><i>Y</i></span>. In the next line output <span class="tex-span"><i>m</i></span> distinct space-separated integers <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>), such that the required equality holds. The sets <span class="tex-span"><i>X</i></span> and <span class="tex-span"><i>Y</i></span> should not intersect, i.e. <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>j</i></sub></span> for all <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>; <span class="tex-span">1 ≤ <i>j</i> ≤ <i>m</i></span>). It is guaranteed that at least one solution always exists. If there are multiple solutions, output any of them.</p></div>

## Input

<p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>), the number of blocks in the set <span class="tex-span"><i>X</i></span>. The next line contains <span class="tex-span"><i>n</i></span> distinct space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>), the numbers of the blocks in <span class="tex-span"><i>X</i></span>.</p><p><span class="tex-font-style-bf">Note</span>: since the size of the input and output could be very large, don't use slow output techniques in your language. For example, do not use input and output streams (cin, cout) in C++.</p>

## Output

<p>In the first line of output print a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup> - <i>n</i></span>), the number of blocks in the set <span class="tex-span"><i>Y</i></span>. In the next line output <span class="tex-span"><i>m</i></span> distinct space-separated integers <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>), such that the required equality holds. The sets <span class="tex-span"><i>X</i></span> and <span class="tex-span"><i>Y</i></span> should not intersect, i.e. <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>j</i></sub></span> for all <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>; <span class="tex-span">1 ≤ <i>j</i> ≤ <i>m</i></span>). It is guaranteed that at least one solution always exists. If there are multiple solutions, output any of them.</p>





```input1
3
1 4 5

```




```input2
1
1

```




```output1
2
999993 1000000
```




```output2
1
1000000 

```


