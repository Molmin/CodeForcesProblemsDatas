## Description

<div><p>The Little Elephant loves permutations of integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> very much. But most of all he loves sorting them. To sort a permutation, the Little Elephant repeatedly swaps some elements. As a result, he must receive a permutation <span class="tex-span">1, 2, 3, ..., <i>n</i></span>.</p><p>This time the Little Elephant has permutation <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span>. Its sorting program needs to make exactly <span class="tex-span"><i>m</i></span> moves, during the <span class="tex-span"><i>i</i></span>-th move it swaps elements that are at that moment located at the <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>-th and the <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>-th positions. But the Little Elephant's sorting program happened to break down and now on every step it can equiprobably either do nothing or swap the required elements.</p><p>Now the Little Elephant doesn't even hope that the program will sort the permutation, but he still wonders: if he runs the program and gets some permutation, how much will the result of sorting resemble the sorted one? For that help the Little Elephant find the mathematical expectation of the number of permutation inversions after all moves of the program are completed.</p><p>We'll call a pair of integers <span class="tex-span"><i>i</i>, <i>j</i></span> <span class="tex-span">(1 ≤ <i>i</i> &lt; <i>j</i> ≤ <i>n</i>)</span> an <span class="tex-font-style-it">inversion</span> in permutatuon <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span>, if the following inequality holds: <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> &gt; <i>p</i><sub class="lower-index"><i>j</i></sub></span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 1000, <i>n</i> &gt; 1)</span> — the permutation size and the number of moves. The second line contains <span class="tex-span"><i>n</i></span> distinct integers, not exceeding <span class="tex-span"><i>n</i></span> — the initial permutation. Next <span class="tex-span"><i>m</i></span> lines each contain two integers: the <span class="tex-span"><i>i</i></span>-th line contains integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> — the positions of elements that were changed during the <span class="tex-span"><i>i</i></span>-th move.</p></div><div class="output-specification"><p>In the only line print a single real number — the answer to the problem. The answer will be considered correct if its relative or absolute error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 1000, <i>n</i> &gt; 1)</span> — the permutation size and the number of moves. The second line contains <span class="tex-span"><i>n</i></span> distinct integers, not exceeding <span class="tex-span"><i>n</i></span> — the initial permutation. Next <span class="tex-span"><i>m</i></span> lines each contain two integers: the <span class="tex-span"><i>i</i></span>-th line contains integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> — the positions of elements that were changed during the <span class="tex-span"><i>i</i></span>-th move.</p>

## Output

<p>In the only line print a single real number — the answer to the problem. The answer will be considered correct if its relative or absolute error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
2 1
1 2
1 2

```




```input2
4 3
1 3 2 4
1 2
2 3
1 4

```




```output1
0.500000000

```




```output2
3.000000000

```


