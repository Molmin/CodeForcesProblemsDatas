## Description

<div><p>Iahub wants to enhance his multitasking abilities. In order to do this, he wants to sort <span class="tex-span"><i>n</i></span> arrays simultaneously, each array consisting of <span class="tex-span"><i>m</i></span> integers.</p><p>Iahub can choose a pair of distinct indices <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> <span class="tex-span">(1 ≤ <i>i</i>, <i>j</i> ≤ <i>m</i>, <i>i</i> ≠ <i>j</i>)</span>. Then in each array the values at positions <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> are swapped only if the value at position <span class="tex-span"><i>i</i></span> is strictly greater than the value at position <span class="tex-span"><i>j</i></span>.</p><p>Iahub wants to find an array of pairs of distinct indices that, chosen in order, sort all of the <span class="tex-span"><i>n</i></span> arrays in ascending or descending order (the particular order is given in input). The size of the array can be at most <img align="middle" class="tex-formula" src="file://o22PF9gK.png" style="max-width: 100.0%;max-height: 100.0%;"> (at most <img align="middle" class="tex-formula" src="file://zOkBsdAy.png" style="max-width: 100.0%;max-height: 100.0%;"> pairs). Help Iahub, find any suitable array.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤  <i>n</i> ≤ 1000)</span>, <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤  100)</span> and <span class="tex-span"><i>k</i></span>. Integer <span class="tex-span"><i>k</i></span> is <span class="tex-span">0</span> if the arrays must be sorted in ascending order, and <span class="tex-span">1</span> if the arrays must be sorted in descending order. Each line <span class="tex-span"><i>i</i></span> of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> integers separated by a space, representing the <span class="tex-span"><i>i</i></span>-th array. For each element <span class="tex-span"><i>x</i></span> of the array <span class="tex-span"><i>i</i></span>, <span class="tex-span">1 ≤ <i>x</i> ≤ 10<sup class="upper-index">6</sup></span> holds.</p></div><div class="output-specification"><p>On the first line of the output print an integer <span class="tex-span"><i>p</i></span>, the size of the array (<span class="tex-span"><i>p</i></span> can be at most <img align="middle" class="tex-formula" src="file://239Rxui3.png" style="max-width: 100.0%;max-height: 100.0%;">). Each of the next <span class="tex-span"><i>p</i></span> lines must contain two distinct integers <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> <span class="tex-span">(1 ≤ <i>i</i>, <i>j</i> ≤ <i>m</i>, <i>i</i> ≠ <i>j</i>)</span>, representing the chosen indices.</p><p>If there are multiple correct answers, you can print any.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤  <i>n</i> ≤ 1000)</span>, <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤  100)</span> and <span class="tex-span"><i>k</i></span>. Integer <span class="tex-span"><i>k</i></span> is <span class="tex-span">0</span> if the arrays must be sorted in ascending order, and <span class="tex-span">1</span> if the arrays must be sorted in descending order. Each line <span class="tex-span"><i>i</i></span> of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> integers separated by a space, representing the <span class="tex-span"><i>i</i></span>-th array. For each element <span class="tex-span"><i>x</i></span> of the array <span class="tex-span"><i>i</i></span>, <span class="tex-span">1 ≤ <i>x</i> ≤ 10<sup class="upper-index">6</sup></span> holds.</p>

## Output

<p>On the first line of the output print an integer <span class="tex-span"><i>p</i></span>, the size of the array (<span class="tex-span"><i>p</i></span> can be at most <img align="middle" class="tex-formula" src="file://239Rxui3.png" style="max-width: 100.0%;max-height: 100.0%;">). Each of the next <span class="tex-span"><i>p</i></span> lines must contain two distinct integers <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> <span class="tex-span">(1 ≤ <i>i</i>, <i>j</i> ≤ <i>m</i>, <i>i</i> ≠ <i>j</i>)</span>, representing the chosen indices.</p><p>If there are multiple correct answers, you can print any.</p>





```input1
2 5 0
1 3 2 5 4
1 4 3 2 5

```




```input2
3 2 1
1 2
2 3
3 4

```




```output1
3
2 4
2 3
4 5

```




```output2
1
2 1

```



## Note

<p>Consider the first sample. After the first operation, the arrays become <span class="tex-span">[1, 3, 2, 5, 4]</span> and <span class="tex-span">[1, 2, 3, 4, 5]</span>. After the second operation, the arrays become <span class="tex-span">[1, 2, 3, 5, 4]</span> and <span class="tex-span">[1, 2, 3, 4, 5]</span>. After the third operation they become <span class="tex-span">[1, 2, 3, 4, 5]</span> and <span class="tex-span">[1, 2, 3, 4, 5]</span>.</p>
