## Description

<div><p>Programming teacher Dmitry Olegovich is going to propose the following task for one of his tests for students:</p><p>You are given a tree <span class="tex-span"><i>T</i></span> with <span class="tex-span"><i>n</i></span> vertices, specified by its adjacency matrix <span class="tex-span"><i>a</i>[1... <i>n</i>, 1... <i>n</i>]</span>. What is the output of the following pseudocode?</p><pre class="verbatim"><br>used[1 ... n] = {0, ..., 0};<br><br>procedure dfs(v):<br>    print v;<br>    used[v] = 1;<br>    for i = 1, 2, ..., n:<br>        if (a[v][i] == 1 and used[i] == 0):<br>            dfs(i);<br><br>dfs(1);<br></pre><p>In order to simplify the test results checking procedure, Dmitry Olegovich decided to create a tree <span class="tex-span"><i>T</i></span> such that the result is his favorite sequence <span class="tex-span"><i>b</i></span>. On the other hand, Dmitry Olegovich doesn't want to provide students with same trees as input, otherwise they might cheat. That's why Dmitry Olegovich is trying to find out the number of different trees <span class="tex-span"><i>T</i></span> such that the result of running the above pseudocode with <span class="tex-span"><i>T</i></span> as input is exactly the sequence <span class="tex-span"><i>b</i></span>. Can you help him?</p><p>Two trees with <span class="tex-span"><i>n</i></span> vertices are called different if their adjacency matrices <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span> are different, i. e. there exists a pair <span class="tex-span">(<i>i</i>, <i>j</i>)</span>, such that <span class="tex-span">1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i></span> and <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>[<i>i</i>][<i>j</i>] ≠ <i>a</i><sub class="lower-index">2</sub>[<i>i</i>][<i>j</i>]</span>.</p></div><div class="input-specification"><p>The first line contains the positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500</span>) — the length of sequence <span class="tex-span"><i>b</i></span>. </p><p>The second line contains <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). It is guaranteed that <span class="tex-span"><i>b</i></span> is a permutation, or in other words, each of the numbers <span class="tex-span">1, 2, ..., <i>n</i></span> appears exactly once in the sequence <span class="tex-span"><i>b</i></span>. Also it is guaranteed that <span class="tex-span"><i>b</i><sub class="lower-index">1</sub> = 1</span>.</p></div><div class="output-specification"><p>Output the number of trees satisfying the conditions above modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line contains the positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500</span>) — the length of sequence <span class="tex-span"><i>b</i></span>. </p><p>The second line contains <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). It is guaranteed that <span class="tex-span"><i>b</i></span> is a permutation, or in other words, each of the numbers <span class="tex-span">1, 2, ..., <i>n</i></span> appears exactly once in the sequence <span class="tex-span"><i>b</i></span>. Also it is guaranteed that <span class="tex-span"><i>b</i><sub class="lower-index">1</sub> = 1</span>.</p>

## Output

<p>Output the number of trees satisfying the conditions above modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
3
1 2 3

```




```input2
3
1 3 2

```




```output1
2

```




```output2
1

```


