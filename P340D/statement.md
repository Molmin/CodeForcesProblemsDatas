## Description

<div><p>Iahub recently has learned Bubble Sort, an algorithm that is used to sort a permutation with <span class="tex-span"><i>n</i></span> elements <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> in ascending order. He is bored of this so simple algorithm, so he invents his own graph. The graph (let's call it <span class="tex-span"><i>G</i></span>) initially has <span class="tex-span"><i>n</i></span> vertices and 0 edges. During Bubble Sort execution, edges appear as described in the following algorithm (pseudocode). </p><pre class="verbatim"><br>procedure bubbleSortGraph()<br>    build a graph G with n vertices and 0 edges<br>    repeat<br>        swapped = false<br>        for i = 1 to n - 1 inclusive do:<br>            if a[i] &gt; a[i + 1] then<br>                add an undirected edge in G between a[i] and a[i + 1]<br>                swap( a[i], a[i + 1] )<br>                swapped = true<br>            end if<br>        end for<br>    until not swapped <br>    /* repeat the algorithm as long as swapped value is true. */ <br>end procedure<br></pre><p>For a graph, an independent set is a set of vertices in a graph, no two of which are adjacent (so there are no edges between vertices of an independent set). A maximum independent set is an independent set which has maximum cardinality. Given the permutation, find the size of the maximum independent set of graph <span class="tex-span"><i>G</i></span>, if we use such permutation as the premutation <span class="tex-span"><i>a</i></span> in procedure bubbleSortGraph.</p></div><div class="input-specification"><p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The next line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>.</p></div><div class="output-specification"><p>Output a single integer — the answer to the problem. </p></div>

## Input

<p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The next line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>.</p>

## Output

<p>Output a single integer — the answer to the problem. </p>





```input1
3
3 1 2

```




```output1
2

```



## Note

<p>Consider the first example. Bubble sort swaps elements 3 and 1. We add edge (1, 3). Permutation is now [1, 3, 2]. Then bubble sort swaps elements 3 and 2. We add edge (2, 3). Permutation is now sorted. We have a graph with 3 vertices and 2 edges (1, 3) and (2, 3). Its maximal independent set is [1, 2].</p>
