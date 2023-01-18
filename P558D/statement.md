## Description

<div><p>Amr bought a new video game "Guess Your Way Out! II". The goal of the game is to find an exit from the maze that looks like a perfect binary tree of height <span class="tex-span"><i>h</i></span>. The player is initially standing at the root of the tree and the exit from the tree is located at some leaf node.</p><p>Let's index all the nodes of the tree such that </p><ul> <li> The root is number <span class="tex-span">1</span> </li><li> Each internal node <span class="tex-span"><i>i</i></span> (<span class="tex-span"><i>i</i> ≤ 2<sup class="upper-index"><i>h</i> - 1</sup> - 1</span>) will have a left child with index = <span class="tex-span">2<i>i</i></span> and a right child with index = <span class="tex-span">2<i>i</i> + 1</span> </li></ul><p>The level of a node is defined as <span class="tex-span">1</span> for a root, or <span class="tex-span">1</span> + level of parent of the node otherwise. The vertices of the level <span class="tex-span"><i>h</i></span> are called leaves. The exit to the maze is located at some leaf node <span class="tex-span"><i>n</i></span>, the player doesn't know where the exit is so he has to guess his way out! </p><p>In the new version of the game the player is allowed to ask questions on the format "Does the <span class="tex-span"><i>ancestor</i>(<i>exit</i>, <i>i</i>)</span> node number belong to the range <span class="tex-span">[<i>L</i>, <i>R</i>]</span>?". Here <span class="tex-span"><i>ancestor</i>(<i>v</i>, <i>i</i>)</span> is the ancestor of a node <span class="tex-span"><i>v</i></span> that located in the level <span class="tex-span"><i>i</i></span>. The game will answer with "Yes" or "No" only. The game is designed such that it doesn't always answer correctly, and sometimes it cheats to confuse the player!.</p><p>Amr asked a lot of questions and got confused by all these answers, so he asked you to help him. Given the questions and its answers, can you identify whether the game is telling contradictory information or not? If the information is not contradictory and the exit node can be determined uniquely, output its number. If the information is not contradictory, but the exit node isn't defined uniquely, output that the number of questions is not sufficient. Otherwise output that the information is contradictory.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>h</i>, <i>q</i></span> (<span class="tex-span">1 ≤ <i>h</i> ≤ 50</span>, <span class="tex-span">0 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>), the height of the tree and the number of questions respectively.</p><p>The next <span class="tex-span"><i>q</i></span> lines will contain four integers each <span class="tex-span"><i>i</i>, <i>L</i>, <i>R</i>, <i>ans</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>h</i></span>, <span class="tex-span">2<sup class="upper-index"><i>i</i> - 1</sup> ≤ <i>L</i> ≤ <i>R</i> ≤ 2<sup class="upper-index"><i>i</i></sup> - 1</span>, <img align="middle" class="tex-formula" src="file://QRUTXEb7.png" style="max-width: 100.0%;max-height: 100.0%;">), representing a question as described in the statement with its answer (<span class="tex-span"><i>ans</i> = 1</span> if the answer is "Yes" and <span class="tex-span"><i>ans</i> = 0</span> if the answer is "No").</p></div><div class="output-specification"><p>If the information provided by the game is contradictory output "Game cheated!" without the quotes.</p><p>Else if you can uniquely identify the exit to the maze output its index. </p><p>Otherwise output "Data not sufficient!" without the quotes.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>h</i>, <i>q</i></span> (<span class="tex-span">1 ≤ <i>h</i> ≤ 50</span>, <span class="tex-span">0 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>), the height of the tree and the number of questions respectively.</p><p>The next <span class="tex-span"><i>q</i></span> lines will contain four integers each <span class="tex-span"><i>i</i>, <i>L</i>, <i>R</i>, <i>ans</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>h</i></span>, <span class="tex-span">2<sup class="upper-index"><i>i</i> - 1</sup> ≤ <i>L</i> ≤ <i>R</i> ≤ 2<sup class="upper-index"><i>i</i></sup> - 1</span>, <img align="middle" class="tex-formula" src="file://QRUTXEb7.png" style="max-width: 100.0%;max-height: 100.0%;">), representing a question as described in the statement with its answer (<span class="tex-span"><i>ans</i> = 1</span> if the answer is "Yes" and <span class="tex-span"><i>ans</i> = 0</span> if the answer is "No").</p>

## Output

<p>If the information provided by the game is contradictory output "Game cheated!" without the quotes.</p><p>Else if you can uniquely identify the exit to the maze output its index. </p><p>Otherwise output "Data not sufficient!" without the quotes.</p>





```input1
3 1
3 4 6 0

```




```input2
4 3
4 10 14 1
3 6 6 0
2 3 3 1

```




```input3
4 2
3 4 6 1
4 12 15 1

```




```input4
4 2
3 4 5 1
2 3 3 1

```




```output1
7
```




```output2
14
```




```output3
Data not sufficient!
```




```output4
Game cheated!
```



## Note

<p>Node <span class="tex-span"><i>u</i></span> is an ancestor of node <span class="tex-span"><i>v</i></span> if and only if </p><ul> <li> <span class="tex-span"><i>u</i></span> is the same node as <span class="tex-span"><i>v</i></span>, </li><li> <span class="tex-span"><i>u</i></span> is the parent of node <span class="tex-span"><i>v</i></span>, </li><li> or <span class="tex-span"><i>u</i></span> is an ancestor of the parent of node <span class="tex-span"><i>v</i></span>. </li></ul><p>In the first sample test there are <span class="tex-span">4</span> leaf nodes <span class="tex-span">4, 5, 6, 7</span>. The first question says that the node isn't in the range <span class="tex-span">[4, 6]</span> so the exit is node number <span class="tex-span">7</span>.</p><p>In the second sample test there are <span class="tex-span">8</span> leaf nodes. After the first question the exit is in the range <span class="tex-span">[10, 14]</span>. After the second and the third questions only node number <span class="tex-span">14</span> is correct. Check the picture below to fully understand.</p><p><img class="tex-graphics" src="file://cYV2wpcD.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
