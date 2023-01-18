## Description

<div><p>You are given <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. Find the number of pairs of indexes <span class="tex-span"><i>i</i>, <i>j</i></span> (<span class="tex-span"><i>i</i> &lt; <i>j</i></span>) that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> + <i>a</i><sub class="lower-index"><i>j</i></sub></span> is a power of <span class="tex-span">2</span> (i. e. some integer <span class="tex-span"><i>x</i></span> exists so that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> + <i>a</i><sub class="lower-index"><i>j</i></sub> = 2<sup class="upper-index"><i>x</i></sup></span>).</p></div><div class="input-specification"><p>The first line contains the single positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of integers.</p><p>The second line contains <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print the number of pairs of indexes <span class="tex-span"><i>i</i>, <i>j</i></span> (<span class="tex-span"><i>i</i> &lt; <i>j</i></span>) that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> + <i>a</i><sub class="lower-index"><i>j</i></sub></span> is a power of <span class="tex-span">2</span>.</p></div>

## Input

<p>The first line contains the single positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of integers.</p><p>The second line contains <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print the number of pairs of indexes <span class="tex-span"><i>i</i>, <i>j</i></span> (<span class="tex-span"><i>i</i> &lt; <i>j</i></span>) that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> + <i>a</i><sub class="lower-index"><i>j</i></sub></span> is a power of <span class="tex-span">2</span>.</p>





```input1
4
7 3 2 1

```




```input2
3
1 1 1

```




```output1
2

```




```output2
3

```



## Note

<p>In the first example the following pairs of indexes include in answer: <span class="tex-span">(1, 4)</span> and <span class="tex-span">(2, 4)</span>.</p><p>In the second example all pairs of indexes <span class="tex-span">(<i>i</i>, <i>j</i>)</span> (where <span class="tex-span"><i>i</i> &lt; <i>j</i></span>) include in answer.</p>
