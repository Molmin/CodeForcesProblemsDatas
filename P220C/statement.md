## Description

<div><p>The Little Elephant has two permutations <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> of length <span class="tex-span"><i>n</i></span>, consisting of numbers from 1 to <span class="tex-span"><i>n</i></span>, inclusive. Let's denote the <span class="tex-span"><i>i</i></span>-th <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>n</i>)</span> element of the permutation <span class="tex-span"><i>a</i></span> as <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, the <span class="tex-span"><i>j</i></span>-th <span class="tex-span">(1 ≤ <i>j</i> ≤ <i>n</i>)</span> element of the permutation <span class="tex-span"><i>b</i></span> — as <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span>.</p><p>The <span class="tex-font-style-it">distance</span> between permutations <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> is the minimum absolute value of the difference between the positions of the occurrences of some number in <span class="tex-span"><i>a</i></span> and in <span class="tex-span"><i>b</i></span>. More formally, it's such minimum <span class="tex-span">|<i>i</i> - <i>j</i>|</span>, that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = <i>b</i><sub class="lower-index"><i>j</i></sub></span>.</p><p>A <span class="tex-font-style-it">cyclic shift</span> number <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>n</i>)</span> of permutation <span class="tex-span"><i>b</i></span> consisting from <span class="tex-span"><i>n</i></span> elements is a permutation <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub><i>b</i><sub class="lower-index"><i>i</i> + 1</sub>... <i>b</i><sub class="lower-index"><i>n</i></sub><i>b</i><sub class="lower-index">1</sub><i>b</i><sub class="lower-index">2</sub>... <i>b</i><sub class="lower-index"><i>i</i> - 1</sub></span>. Overall a permutation has <span class="tex-span"><i>n</i></span> cyclic shifts.</p><p>The Little Elephant wonders, for all cyclic shifts of permutation <span class="tex-span"><i>b</i></span>, what is the distance between the cyclic shift and permutation <span class="tex-span"><i>a</i></span>?</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the size of the permutations. The second line contains permutation <span class="tex-span"><i>a</i></span> as <span class="tex-span"><i>n</i></span> distinct numbers from 1 to <span class="tex-span"><i>n</i></span>, inclusive. The numbers are separated with single spaces. The third line contains permutation <span class="tex-span"><i>b</i></span> in the same format.</p></div><div class="output-specification"><p>In <span class="tex-span"><i>n</i></span> lines print <span class="tex-span"><i>n</i></span> integers — the answers for cyclic shifts. Print the answers to the shifts in the order of the shifts' numeration in permutation <span class="tex-span"><i>b</i></span>, that is, first for the 1-st cyclic shift, then for the 2-nd, and so on.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the size of the permutations. The second line contains permutation <span class="tex-span"><i>a</i></span> as <span class="tex-span"><i>n</i></span> distinct numbers from 1 to <span class="tex-span"><i>n</i></span>, inclusive. The numbers are separated with single spaces. The third line contains permutation <span class="tex-span"><i>b</i></span> in the same format.</p>

## Output

<p>In <span class="tex-span"><i>n</i></span> lines print <span class="tex-span"><i>n</i></span> integers — the answers for cyclic shifts. Print the answers to the shifts in the order of the shifts' numeration in permutation <span class="tex-span"><i>b</i></span>, that is, first for the 1-st cyclic shift, then for the 2-nd, and so on.</p>





```input1
2
1 2
2 1

```




```input2
4
2 1 3 4
3 4 2 1

```




```output1
1
0

```




```output2
2
1
0
1

```


