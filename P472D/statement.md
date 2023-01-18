## Description

<div><p>There is an easy way to obtain a new task from an old one called "Inverse the problem": we give an output of the original task, and ask to generate an input, such that solution to the original problem will produce the output we provided. The hard task of Topcoder Open 2014 Round 2C, InverseRMQ, is a good example.</p><p>Now let's create a task this way. We will use the task: you are given a tree, please calculate the distance between any pair of its nodes. Yes, it is very easy, but the inverse version is a bit harder: you are given an <span class="tex-span"><i>n</i> × <i>n</i></span> distance matrix. Determine if it is the distance matrix of a weighted tree (all weights must be positive integers).</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>) — the number of nodes in that graph.</p><p>Then next <span class="tex-span"><i>n</i></span> lines each contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> (<span class="tex-span">0 ≤ <i>d</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the distance between node <span class="tex-span"><i>i</i></span> and node <span class="tex-span"><i>j</i></span>.</p></div><div class="output-specification"><p>If there exists such a tree, output "<span class="tex-font-style-tt">YES</span>", otherwise output "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>) — the number of nodes in that graph.</p><p>Then next <span class="tex-span"><i>n</i></span> lines each contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> (<span class="tex-span">0 ≤ <i>d</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the distance between node <span class="tex-span"><i>i</i></span> and node <span class="tex-span"><i>j</i></span>.</p>

## Output

<p>If there exists such a tree, output "<span class="tex-font-style-tt">YES</span>", otherwise output "<span class="tex-font-style-tt">NO</span>".</p>





```input1
3
0 2 7
2 0 9
7 9 0

```




```input2
3
1 2 7
2 0 9
7 9 0

```




```input3
3
0 2 2
7 0 9
7 9 0

```




```input4
3
0 1 1
1 0 1
1 1 0

```




```input5
2
0 0
0 0

```




```output1
YES

```




```output2
NO

```




```output3
NO

```




```output4
NO

```




```output5
NO

```



## Note

<p>In the first example, the required tree exists. It has one edge between nodes 1 and 2 with weight 2, another edge between nodes 1 and 3 with weight 7.</p><p>In the second example, it is impossible because <span class="tex-span"><i>d</i><sub class="lower-index">1, 1</sub></span> should be 0, but it is 1.</p><p>In the third example, it is impossible because <span class="tex-span"><i>d</i><sub class="lower-index">1, 2</sub></span> should equal <span class="tex-span"><i>d</i><sub class="lower-index">2, 1</sub></span>.</p>
