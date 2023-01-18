## Description

<div><p><span class="tex-font-style-underline">Petya loves lucky numbers. We all know that lucky numbers are the positive integers whose decimal representations contain only the lucky digits <span class="tex-font-style-bf">4</span> and <span class="tex-font-style-bf">7</span>. For example, numbers <span class="tex-font-style-bf">47</span>, <span class="tex-font-style-bf">744</span>, <span class="tex-font-style-bf">4</span> are lucky and <span class="tex-font-style-bf">5</span>, <span class="tex-font-style-bf">17</span>, <span class="tex-font-style-bf">467</span> are not.</span></p><p>One day Petya encountered a tree with <span class="tex-span"><i>n</i></span> vertexes. Besides, the tree was weighted, i. e. each edge of the tree has weight (a positive integer). An edge is lucky if its weight is a lucky number. Note that a <span class="tex-font-style-underline">tree with <span class="tex-span"><i>n</i></span> vertexes</span> is an undirected connected graph that has exactly <span class="tex-span"><i>n</i> - 1</span> edges.</p><p>Petya wondered how many vertex triples <span class="tex-span">(<i>i</i>, <i>j</i>, <i>k</i>)</span> exists that on the way from <span class="tex-span"><i>i</i></span> to <span class="tex-span"><i>j</i></span>, as well as on the way from <span class="tex-span"><i>i</i></span> to <span class="tex-span"><i>k</i></span> there must be at least one lucky edge (all three vertexes are pairwise distinct). The order of numbers in the triple matters, that is, the triple <span class="tex-span">(1, 2, 3)</span> is not equal to the triple <span class="tex-span">(2, 1, 3)</span> and is not equal to the triple <span class="tex-span">(1, 3, 2)</span>. </p><p>Find how many such triples of vertexes exist.</p></div><div class="input-specification"><p>The first line contains the single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of tree vertexes. Next <span class="tex-span"><i>n</i> - 1</span> lines contain three integers each: <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the pair of vertexes connected by the edge and the edge's weight.</p></div><div class="output-specification"><p>On the single line print the single number — the answer.</p><p>Please do not use the %lld specificator to read or write 64-bit numbers in С++. It is recommended to use the cin, cout streams or the %I64d specificator.</p></div>

## Input

<p>The first line contains the single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of tree vertexes. Next <span class="tex-span"><i>n</i> - 1</span> lines contain three integers each: <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the pair of vertexes connected by the edge and the edge's weight.</p>

## Output

<p>On the single line print the single number — the answer.</p><p>Please do not use the %lld specificator to read or write 64-bit numbers in С++. It is recommended to use the cin, cout streams or the %I64d specificator.</p>





```input1
4
1 2 4
3 1 2
1 4 7

```




```input2
4
1 2 4
1 3 47
1 4 7447

```




```output1
16

```




```output2
24

```



## Note

<p>The <span class="tex-span">16</span> triples of vertexes from the first sample are: <span class="tex-span">(1, 2, 4), (1, 4, 2), (2, 1, 3), (2, 1, 4), (2, 3, 1), (2, 3, 4), (2, 4, 1), (2, 4, 3), (3, 2, 4), (3, 4, 2), (4, 1, 2), (4, 1, 3), (4, 2, 1), (4, 2, 3), (4, 3, 1), (4, 3, 2)</span>.</p><p>In the second sample all the triples should be counted: <span class="tex-span">4·3·2 = 24</span>.</p>
