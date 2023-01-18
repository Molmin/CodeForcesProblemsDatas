## Description

<div><p>Polycarpus plays with red and blue marbles. He put <span class="tex-span"><i>n</i></span> marbles from the left to the right in a row. As it turned out, the marbles form a <span class="tex-font-style-it">zebroid</span>.</p><p>A non-empty sequence of red and blue marbles is a <span class="tex-font-style-it">zebroid</span>, if the colors of the marbles in this sequence alternate. For example, sequences (<span class="tex-font-style-tt">red; blue; red</span>) and (<span class="tex-font-style-tt">blue</span>) are zebroids and sequence (<span class="tex-font-style-tt">red; red</span>) is not a zebroid.</p><p>Now Polycarpus wonders, how many ways there are to pick a zebroid <span class="tex-font-style-bf">subsequence</span> from this sequence. Help him solve the problem, find the number of ways modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>)</span> — the number of marbles in Polycarpus's sequence.</p></div><div class="output-specification"><p>Print a single number — the answer to the problem modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>)</span> — the number of marbles in Polycarpus's sequence.</p>

## Output

<p>Print a single number — the answer to the problem modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
3

```




```input2
4

```




```output1
6

```




```output2
11

```



## Note

<p>Let's consider the first test sample. Let's assume that Polycarpus initially had sequence (<span class="tex-font-style-tt">red; blue; red</span>), so there are six ways to pick a zebroid: </p><ul> <li> pick the first marble; </li><li> pick the second marble; </li><li> pick the third marble; </li><li> pick the first and second marbles; </li><li> pick the second and third marbles; </li><li> pick the first, second and third marbles. </li></ul><p>It can be proven that if Polycarpus picks (<span class="tex-font-style-tt">blue; red; blue</span>) as the initial sequence, the number of ways won't change.</p>
