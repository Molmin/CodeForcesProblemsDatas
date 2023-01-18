## Description

<div><p><span class="tex-font-style-it">Hands that shed innocent blood!</span></p><p>There are <span class="tex-span"><i>n</i></span> guilty people in a line, the <span class="tex-span"><i>i</i></span>-th of them holds a claw with length <span class="tex-span"><i>L</i><sub class="lower-index"><i>i</i></sub></span>. The bell rings and every person kills some of people in front of him. All people kill others at the same time. Namely, the <span class="tex-span"><i>i</i></span>-th person kills the <span class="tex-span"><i>j</i></span>-th person if and only if <span class="tex-span"><i>j</i> &lt; <i>i</i></span> and <span class="tex-span"><i>j</i> ≥ <i>i</i> - <i>L</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>You are given lengths of the claws. You need to find the total number of alive people after the bell rings.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of guilty people.</p><p>Second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>L</i><sub class="lower-index">1</sub>, <i>L</i><sub class="lower-index">2</sub>, ..., <i>L</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>L</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>L</i><sub class="lower-index"><i>i</i></sub></span> is the length of the <span class="tex-span"><i>i</i></span>-th person's claw.</p></div><div class="output-specification"><p>Print one integer — the total number of alive people after the bell rings.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of guilty people.</p><p>Second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>L</i><sub class="lower-index">1</sub>, <i>L</i><sub class="lower-index">2</sub>, ..., <i>L</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>L</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>L</i><sub class="lower-index"><i>i</i></sub></span> is the length of the <span class="tex-span"><i>i</i></span>-th person's claw.</p>

## Output

<p>Print one integer — the total number of alive people after the bell rings.</p>





```input1
4
0 1 0 10

```




```input2
2
0 0

```




```input3
10
1 1 3 0 0 0 2 1 0 3

```




```output1
1

```




```output2
2

```




```output3
3

```



## Note

<p>In first sample the last person kills everyone in front of him.</p>
