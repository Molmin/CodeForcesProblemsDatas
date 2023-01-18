## Description

<div><p>After destroying all of Voldemort's Horcruxes, Harry and Voldemort are up for the final battle. They each cast spells from their wands and the spells collide.</p><p>The battle scene is Hogwarts, which can be represented in the form of a tree. There are, in total, <span class="tex-span"><i>n</i></span> places in Hogwarts joined using <span class="tex-span"><i>n</i> - 1</span> undirected roads.</p><p>Ron, who was viewing this battle between Harry and Voldemort, wondered how many triplets of places <span class="tex-span">(<i>u</i>, <i>v</i>, <i>w</i>)</span> are there such that if Harry is standing at place <span class="tex-span"><i>u</i></span> and Voldemort is standing at place <span class="tex-span"><i>v</i></span>, their spells collide at a place <span class="tex-span"><i>w</i></span>. This is possible for a triplet only when <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>w</i></span> are distinct, and there exist paths from <span class="tex-span"><i>u</i></span> to <span class="tex-span"><i>w</i></span> and from <span class="tex-span"><i>v</i></span> to <span class="tex-span"><i>w</i></span> which do not pass through the same roads.</p><p>Now, due to the battle havoc, new paths are being added all the time. You have to tell Ron the answer after each addition.</p><p>Formally, you are given a tree with <span class="tex-span"><i>n</i></span> vertices and <span class="tex-span"><i>n</i> - 1</span> edges. <span class="tex-span"><i>q</i></span> new edges are being added between the nodes of the tree. After each addition you need to tell the number of triplets <span class="tex-span">(<i>u</i>, <i>v</i>, <i>w</i>)</span> such that <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>w</i></span> are distinct and there exist two paths, one between <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>w</i></span>, another between <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>w</i></span> such that these paths do not have an edge in common.</p></div><div class="input-specification"><p>First line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of places in Hogwarts.</p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains two space separated integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>) indicating a road between places <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>. It is guaranteed that the given roads form a connected tree.</p><p>Next line contains a single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of new edges being added.</p><p>Each of the next <span class="tex-span"><i>q</i></span> lines contains two space separated integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>) representing the new road being added.</p><p>Note that it is possible that a newly added road connects places that were connected by a road before. Also, a newly added road may connect a place to itself.</p></div><div class="output-specification"><p>In the first line print the value for the number of triplets before any changes occurred.</p><p>After that print <span class="tex-span"><i>q</i></span> lines, a single integer <span class="tex-span"><i>ans</i><sub class="lower-index"><i>i</i></sub></span> in each line containing the value for the number of triplets after <span class="tex-span"><i>i</i></span>-th edge addition.</p></div>

## Input

<p>First line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of places in Hogwarts.</p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains two space separated integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>) indicating a road between places <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>. It is guaranteed that the given roads form a connected tree.</p><p>Next line contains a single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of new edges being added.</p><p>Each of the next <span class="tex-span"><i>q</i></span> lines contains two space separated integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>) representing the new road being added.</p><p>Note that it is possible that a newly added road connects places that were connected by a road before. Also, a newly added road may connect a place to itself.</p>

## Output

<p>In the first line print the value for the number of triplets before any changes occurred.</p><p>After that print <span class="tex-span"><i>q</i></span> lines, a single integer <span class="tex-span"><i>ans</i><sub class="lower-index"><i>i</i></sub></span> in each line containing the value for the number of triplets after <span class="tex-span"><i>i</i></span>-th edge addition.</p>





```input1
3
1 2
2 3
1
2 3

```




```input2
4
1 2
2 3
2 4
2
1 4
3 4

```




```input3
5
1 2
2 3
3 4
4 5
1
1 5

```




```output1
2
4

```




```output2
6
18
24

```




```output3
20
60

```



## Note

<p>In the first sample case, for the initial tree, we have <span class="tex-span">(1, 3, 2)</span> and <span class="tex-span">(3, 1, 2)</span> as the only possible triplets <span class="tex-span">(<i>u</i>, <i>v</i>, <i>w</i>)</span>.</p><p>After addition of edge from <span class="tex-span">2</span> to <span class="tex-span">3</span>, we have <span class="tex-span">(1, 3, 2)</span>, <span class="tex-span">(3, 1, 2)</span>, <span class="tex-span">(1, 2, 3)</span> and <span class="tex-span">(2, 1, 3)</span> as the possible triplets.</p>
