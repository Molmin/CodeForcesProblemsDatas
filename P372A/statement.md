## Description

<div><p>There are <span class="tex-span"><i>n</i></span> kangaroos with pockets. Each kangaroo has a size (integer number). A kangaroo can go into another kangaroo's pocket if and only if the size of kangaroo who hold the kangaroo is at least twice as large as the size of kangaroo who is held.</p><p>Each kangaroo can hold at most one kangaroo, and the kangaroo who is held by another kangaroo cannot hold any kangaroos.</p><p>The kangaroo who is held by another kangaroo cannot be visible from outside. Please, find a plan of holding kangaroos with the minimal number of kangaroos who is visible.</p></div><div class="input-specification"><p>The first line contains a single integer — <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup>)</span>. Each of the next <span class="tex-span"><i>n</i></span> lines contains an integer <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> — the size of the <span class="tex-span"><i>i</i></span>-th kangaroo <span class="tex-span">(1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span>.</p></div><div class="output-specification"><p>Output a single integer — the optimal number of visible kangaroos.</p></div>

## Input

<p>The first line contains a single integer — <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup>)</span>. Each of the next <span class="tex-span"><i>n</i></span> lines contains an integer <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> — the size of the <span class="tex-span"><i>i</i></span>-th kangaroo <span class="tex-span">(1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span>.</p>

## Output

<p>Output a single integer — the optimal number of visible kangaroos.</p>





```input1
8
2
5
7
6
9
8
4
2

```




```input2
8
9
1
6
2
6
5
8
3

```




```output1
5

```




```output2
5

```


