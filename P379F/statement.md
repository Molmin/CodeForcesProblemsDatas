## Description

<div><p>You are a programmer and you have a New Year Tree (not the traditional fur tree, though) — a tree of four vertices: one vertex of degree three (has number 1), connected with three leaves (their numbers are from 2 to 4).</p><p>On the New Year, programmers usually have fun. You decided to have fun as well by adding vertices to the tree. One adding operation looks as follows:</p><ul> <li> First we choose some leaf of the tree with number <span class="tex-span"><i>v</i></span>. </li><li> Let's mark the number of vertices on the tree at this moment by variable <span class="tex-span"><i>n</i></span>, then two vertexes are added to the tree, their numbers are <span class="tex-span"><i>n</i> + 1</span> and <span class="tex-span"><i>n</i> + 2</span>, also you get new edges, one between vertices <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>n</i> + 1</span> and one between vertices <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>n</i> + 2</span>. </li></ul><p>Your task is not just to model the process of adding vertices to the tree, but after each adding operation print the diameter of the current tree. Come on, let's solve the New Year problem!</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>q</i></span> <span class="tex-span">(1 ≤ <i>q</i> ≤ 5·10<sup class="upper-index">5</sup>)</span> — the number of operations. Each of the next <span class="tex-span"><i>q</i></span> lines contains integer <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the operation of adding leaves to vertex <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. Variable <span class="tex-span"><i>n</i></span> represents the number of vertices in the current tree.</p><p>It is guaranteed that all given operations are correct.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>q</i></span> integers — the diameter of the current tree after each operation.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>q</i></span> <span class="tex-span">(1 ≤ <i>q</i> ≤ 5·10<sup class="upper-index">5</sup>)</span> — the number of operations. Each of the next <span class="tex-span"><i>q</i></span> lines contains integer <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the operation of adding leaves to vertex <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. Variable <span class="tex-span"><i>n</i></span> represents the number of vertices in the current tree.</p><p>It is guaranteed that all given operations are correct.</p>

## Output

<p>Print <span class="tex-span"><i>q</i></span> integers — the diameter of the current tree after each operation.</p>





```input1
5
2
3
4
8
5

```




```output1
3
4
4
5
6

```


