## Description

<div><p>Mahmoud was trying to solve the vertex cover problem on trees. The problem statement is:</p><p>Given an undirected tree consisting of <span class="tex-span"><i>n</i></span> nodes, find the minimum number of vertices that cover all the edges. Formally, we need to find a set of vertices such that for each edge <span class="tex-span">(<i>u</i>, <i>v</i>)</span> that belongs to the tree, either <span class="tex-span"><i>u</i></span> is in the set, or <span class="tex-span"><i>v</i></span> is in the set, <span class="tex-font-style-bf">or both are in the set</span>. Mahmoud has found the following algorithm:</p><ul> <li> Root the tree at node <span class="tex-span">1</span>. </li><li> Count the number of nodes at an even depth. Let it be <span class="tex-span"><i>evenCnt</i></span>. </li><li> Count the number of nodes at an odd depth. Let it be <span class="tex-span"><i>oddCnt</i></span>. </li><li> The answer is the minimum between <span class="tex-span"><i>evenCnt</i></span> and <span class="tex-span"><i>oddCnt</i></span>. </li></ul><p>The depth of a node in a tree is the number of edges in the shortest path between this node and the root. The depth of the root is 0.</p><p>Ehab told Mahmoud that this algorithm is wrong, but he didn't believe because he had tested his algorithm against many trees and it worked, so Ehab asked you to find 2 trees consisting of <span class="tex-span"><i>n</i></span> nodes. The algorithm should find an incorrect answer for the first tree and a correct answer for the second one.</p></div><div class="input-specification"><p>The only line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>, the number of nodes in the desired trees.</p></div><div class="output-specification"><p>The output should consist of 2 <span class="tex-font-style-bf">independent</span> sections, each containing a tree. The algorithm should find an incorrect answer for the tree in the first section and a correct answer for the tree in the second. If a tree doesn't exist for some section, output "-1" (without quotes) <span class="tex-font-style-bf">for that section only</span>.</p><p>If the answer for a section exists, it should contain <span class="tex-span"><i>n</i> - 1</span> lines, each containing 2 space-separated integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> <span class="tex-span">(1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i>)</span>, which means that there's an undirected edge between node <span class="tex-span"><i>u</i></span> and node <span class="tex-span"><i>v</i></span>. If the given graph isn't a tree or it doesn't follow the format, you'll receive wrong answer verdict.</p><p>If there are multiple answers, you can print any of them.</p></div>

## Input

<p>The only line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>, the number of nodes in the desired trees.</p>

## Output

<p>The output should consist of 2 <span class="tex-font-style-bf">independent</span> sections, each containing a tree. The algorithm should find an incorrect answer for the tree in the first section and a correct answer for the tree in the second. If a tree doesn't exist for some section, output "-1" (without quotes) <span class="tex-font-style-bf">for that section only</span>.</p><p>If the answer for a section exists, it should contain <span class="tex-span"><i>n</i> - 1</span> lines, each containing 2 space-separated integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> <span class="tex-span">(1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i>)</span>, which means that there's an undirected edge between node <span class="tex-span"><i>u</i></span> and node <span class="tex-span"><i>v</i></span>. If the given graph isn't a tree or it doesn't follow the format, you'll receive wrong answer verdict.</p><p>If there are multiple answers, you can print any of them.</p>





```input1
2

```




```input2
8

```




```output1
-1
1 2

```




```output2
1 2
1 3
2 4
2 5
3 6
4 7
4 8
1 2
1 3
2 4
2 5
2 6
3 7
6 8
```



## Note

<p>In the first sample, there is only 1 tree with 2 nodes (node <span class="tex-span">1</span> connected to node <span class="tex-span">2</span>). The algorithm will produce a correct answer in it so we printed <span class="tex-span"> - 1</span> in the first section, but notice that we printed this tree in the second section.</p><p>In the second sample:</p><p>In the first tree, the algorithm will find an answer with 4 nodes, while there exists an answer with 3 nodes like this: <img class="tex-graphics" src="file://Ml3zu4Ue.png" style="max-width: 100.0%;max-height: 100.0%;"> In the second tree, the algorithm will find an answer with 3 nodes which is correct: <img class="tex-graphics" src="file://pVymIgtu.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
