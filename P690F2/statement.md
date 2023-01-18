## Description

<div><p>Heidi got tired of deciphering the prophecy hidden in the Tree of Life and decided to go back to her headquarters, rest a little and try there. Of course, she cannot uproot the Tree and take it with her, so she made a drawing of the Tree on a piece of paper. On second thought, she made more identical drawings so as to have <span class="tex-span"><i>n</i></span> in total (where <span class="tex-span"><i>n</i></span> is the number of vertices of the Tree of Life) – who knows what might happen?</p><p>Indeed, on her way back Heidi was ambushed by a group of zombies. While she managed to fend them off, they have damaged her drawings in a peculiar way: from the <span class="tex-span"><i>i</i></span>-th copy, the vertex numbered <span class="tex-span"><i>i</i></span> was removed, along with all adjacent edges. In each picture, the zombies have also erased all the vertex numbers and relabeled the remaining <span class="tex-span"><i>n</i> - 1</span> vertices arbitrarily using numbers <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> (fortunately, each vertex still has a distinct number). <span class="tex-font-style-it">What's more, the drawings have been arbitrarily shuffled/reordered.</span></p><p>Now Heidi wants to recover the Tree of Life from her descriptions of all the drawings (as lists of edges).</p></div><div class="input-specification"><p>The first line of the input contains <span class="tex-span"><i>Z</i> ≤ 20</span> – the number of test cases. <span class="tex-span"><i>Z</i></span> descriptions of single test cases follow.</p><p>In each test case, the first line of input contains numbers <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>) and <span class="tex-span"><i>k</i></span> (where <span class="tex-span"><i>k</i></span> is the number of drawings; we have <span class="tex-span"><i>k</i> = <i>n</i></span>). In the following lines, the descriptions of the <span class="tex-span"><i>k</i></span> drawings are given. The description of the <span class="tex-span"><i>i</i></span>-th drawing is a line containing <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> – the number of edges in this drawing, followed by <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> lines describing edges, each of which contains two space-separated integers –- the numbers of the two vertices connected by the edge.</p></div><div class="output-specification"><p>If Heidi's drawings cannot possibly come from a single tree, you should output the word <span class="tex-font-style-tt">NO</span>. Otherwise, output one line containing the word <span class="tex-font-style-tt">YES</span> and <span class="tex-span"><i>n</i> - 1</span> lines describing any tree that Heidi's drawings could have come from. For every edge you should output the numbers of the vertices that it connects, separated with a single space. If there are many solutions, print any of them.</p></div>

## Input

<p>The first line of the input contains <span class="tex-span"><i>Z</i> ≤ 20</span> – the number of test cases. <span class="tex-span"><i>Z</i></span> descriptions of single test cases follow.</p><p>In each test case, the first line of input contains numbers <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>) and <span class="tex-span"><i>k</i></span> (where <span class="tex-span"><i>k</i></span> is the number of drawings; we have <span class="tex-span"><i>k</i> = <i>n</i></span>). In the following lines, the descriptions of the <span class="tex-span"><i>k</i></span> drawings are given. The description of the <span class="tex-span"><i>i</i></span>-th drawing is a line containing <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> – the number of edges in this drawing, followed by <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> lines describing edges, each of which contains two space-separated integers –- the numbers of the two vertices connected by the edge.</p>

## Output

<p>If Heidi's drawings cannot possibly come from a single tree, you should output the word <span class="tex-font-style-tt">NO</span>. Otherwise, output one line containing the word <span class="tex-font-style-tt">YES</span> and <span class="tex-span"><i>n</i> - 1</span> lines describing any tree that Heidi's drawings could have come from. For every edge you should output the numbers of the vertices that it connects, separated with a single space. If there are many solutions, print any of them.</p>





```input1
1
5 5
2
4 1
2 1
1
3 1
3
4 1
4 3
2 1
3
3 1
3 2
4 1
3
2 1
3 2
4 2

```




```output1
YES
2 5
4 2
3 2
5 1

```


