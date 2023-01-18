## Description

<div><p>Will shares a psychic connection with the Upside Down Monster, so everything the monster knows, Will knows. Suddenly, he started drawing, page after page, non-stop. Joyce, his mom, and Chief Hopper put the drawings together, and they realized, it's a labeled tree!</p><center> <img class="tex-graphics" src="file://7YFd5LNP.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>A tree is a connected acyclic graph. Will's tree has <span class="tex-span"><i>n</i></span> vertices. Joyce and Hopper don't know what that means, so they're investigating this tree and similar trees. For each <span class="tex-span"><i>k</i></span> such that <span class="tex-span">0 ≤ <i>k</i> ≤ <i>n</i> - 1</span>, they're going to investigate all labeled trees with <span class="tex-span"><i>n</i></span> vertices that share exactly <span class="tex-span"><i>k</i></span> edges with Will's tree. Two labeled trees are different if and only if there's a pair of vertices <span class="tex-span">(<i>v</i>, <i>u</i>)</span> such that there's an edge between <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>u</i></span> in one tree and not in the other one.</p><p>Hopper and Joyce want to know how much work they have to do, so they asked you to tell them the number of labeled trees with <span class="tex-span"><i>n</i></span> vertices that share exactly <span class="tex-span"><i>k</i></span> edges with Will's tree, for each <span class="tex-span"><i>k</i></span>. The answer could be very large, so they only asked you to tell them the answers modulo <span class="tex-span">1000000007 = 10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the size of the tree.</p><p>The next <span class="tex-span"><i>n</i> - 1</span> lines contain the edges of Will's tree. Each line contains two integers <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>u</i></span> (<span class="tex-span">1 ≤ <i>v</i>, <i>u</i> ≤ <i>n</i></span>, <span class="tex-span"><i>v</i> ≠ <i>u</i></span>), endpoints of an edge. It is guaranteed that the given graph is a tree.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> integers in one line. <span class="tex-span"><i>i</i></span>-th integer should be the number of the number of labeled trees with <span class="tex-span"><i>n</i></span> vertices that share exactly <span class="tex-span"><i>i</i> - 1</span> edges with Will's tree, modulo <span class="tex-span">1000 000 007 = 10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the size of the tree.</p><p>The next <span class="tex-span"><i>n</i> - 1</span> lines contain the edges of Will's tree. Each line contains two integers <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>u</i></span> (<span class="tex-span">1 ≤ <i>v</i>, <i>u</i> ≤ <i>n</i></span>, <span class="tex-span"><i>v</i> ≠ <i>u</i></span>), endpoints of an edge. It is guaranteed that the given graph is a tree.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> integers in one line. <span class="tex-span"><i>i</i></span>-th integer should be the number of the number of labeled trees with <span class="tex-span"><i>n</i></span> vertices that share exactly <span class="tex-span"><i>i</i> - 1</span> edges with Will's tree, modulo <span class="tex-span">1000 000 007 = 10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
3
1 2
1 3

```




```input2
4
1 2
2 3
3 4

```




```input3
4
1 2
1 3
1 4

```




```output1
0 2 1
```




```output2
1 7 7 1
```




```output3
0 9 6 1
```


