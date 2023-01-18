## Description

<div><p>Anton loves transforming one permutation into another one by swapping elements for money, and Ira doesn't like paying for stupid games. Help them obtain the required permutation by paying as little money as possible.</p><p>More formally, we have two permutations, <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>s</i></span> of numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. We can swap <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub></span>, by paying <span class="tex-span">|<i>i</i> - <i>j</i>|</span> coins for it. Find and print the smallest number of coins required to obtain permutation <span class="tex-span"><i>s</i></span> from permutation <span class="tex-span"><i>p</i></span>. Also print the sequence of swap operations at which we obtain a solution. </p></div><div class="input-specification"><p>The first line contains a single number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>) — the length of the permutations.</p><p>The second line contains a sequence of <span class="tex-span"><i>n</i></span> numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> — permutation <span class="tex-span"><i>p</i></span>. Each number from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> occurs exactly once in this line.</p><p>The third line contains a sequence of <span class="tex-span"><i>n</i></span> numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> — permutation <span class="tex-span"><i>s</i></span>. Each number from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> occurs once in this line.</p></div><div class="output-specification"><p>In the first line print the minimum number of coins that you need to spend to transform permutation <span class="tex-span"><i>p</i></span> into permutation <span class="tex-span"><i>s</i></span>.</p><p>In the second line print number <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 2·10<sup class="upper-index">6</sup></span>) — the number of operations needed to get the solution.</p><p>In the next <span class="tex-span"><i>k</i></span> lines print the operations. Each line must contain two numbers <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i></span>, <span class="tex-span"><i>i</i> ≠ <i>j</i></span>), which means that you need to swap <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub></span>.</p><p>It is guaranteed that the solution exists.</p></div>

## Input

<p>The first line contains a single number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>) — the length of the permutations.</p><p>The second line contains a sequence of <span class="tex-span"><i>n</i></span> numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> — permutation <span class="tex-span"><i>p</i></span>. Each number from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> occurs exactly once in this line.</p><p>The third line contains a sequence of <span class="tex-span"><i>n</i></span> numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> — permutation <span class="tex-span"><i>s</i></span>. Each number from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> occurs once in this line.</p>

## Output

<p>In the first line print the minimum number of coins that you need to spend to transform permutation <span class="tex-span"><i>p</i></span> into permutation <span class="tex-span"><i>s</i></span>.</p><p>In the second line print number <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 2·10<sup class="upper-index">6</sup></span>) — the number of operations needed to get the solution.</p><p>In the next <span class="tex-span"><i>k</i></span> lines print the operations. Each line must contain two numbers <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i></span>, <span class="tex-span"><i>i</i> ≠ <i>j</i></span>), which means that you need to swap <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub></span>.</p><p>It is guaranteed that the solution exists.</p>





```input1
4
4 2 1 3
3 2 4 1

```




```output1
3
2
4 3
3 1

```



## Note

<p>In the first sample test we swap numbers on positions 3 and 4 and permutation <span class="tex-span"><i>p</i></span> becomes 4 2 3 1. We pay <span class="tex-span">|3 - 4| = 1</span> coins for that. On second turn we swap numbers on positions 1 and 3 and get permutation <span class="tex-span">3241</span> equal to <span class="tex-span"><i>s</i></span>. We pay <span class="tex-span">|3 - 1| = 2</span> coins for that. In total we pay three coins.</p>
