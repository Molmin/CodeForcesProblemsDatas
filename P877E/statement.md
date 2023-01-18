## Description

<div><p>Danil decided to earn some money, so he had found a part-time job. The interview have went well, so now he is a light switcher.</p><p>Danil works in a rooted tree (undirected connected acyclic graph) with <span class="tex-span"><i>n</i></span> vertices, vertex <span class="tex-span">1</span> is the root of the tree. There is a room in each vertex, light can be switched on or off in each room. Danil's duties include switching light in all rooms of the subtree of the vertex. It means that if light is switched on in some room of the subtree, he should switch it off. Otherwise, he should switch it on.</p><p>Unfortunately (or fortunately), Danil is very lazy. He knows that his boss is not going to personally check the work. Instead, he will send Danil tasks using <span class="tex-font-style-tt">Workforces</span> personal messages.</p><p>There are two types of tasks: </p><ol><li> <span class="tex-font-style-tt">pow v</span> describes a task to switch lights in the subtree of vertex <span class="tex-span"><i>v</i></span>.</li><li> <span class="tex-font-style-tt">get v</span> describes a task to count the number of rooms in the subtree of <span class="tex-span"><i>v</i></span>, in which the light is turned on. Danil should send the answer to his boss using <span class="tex-font-style-tt">Workforces</span> messages.</li></ol><p>A subtree of vertex <span class="tex-span"><i>v</i></span> is a set of vertices for which the shortest path from them to the root passes through <span class="tex-span"><i>v</i></span>. In particular, the vertex <span class="tex-span"><i>v</i></span> is in the subtree of <span class="tex-span"><i>v</i></span>.</p><p>Danil is not going to perform his duties. He asks you to write a program, which answers the boss instead of him.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>) — the number of vertices in the tree.</p><p>The second line contains <span class="tex-span"><i>n</i> - 1</span> space-separated integers <span class="tex-span"><i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> &lt; <i>i</i></span>), where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is the ancestor of vertex <span class="tex-span"><i>i</i></span>.</p><p>The third line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>), where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is <span class="tex-span">1</span>, if the light is turned on in vertex <span class="tex-span"><i>i</i></span> and <span class="tex-span">0</span> otherwise.</p><p>The fourth line contains a single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 200 000</span>) — the number of tasks.</p><p>The next <span class="tex-span"><i>q</i></span> lines are <span class="tex-font-style-tt">get v</span> or <span class="tex-font-style-tt">pow v</span> (<span class="tex-span">1 ≤ <i>v</i> ≤ <i>n</i></span>) — the tasks described above.</p></div><div class="output-specification"><p>For each task <span class="tex-font-style-tt">get v</span> print the number of rooms in the subtree of <span class="tex-span"><i>v</i></span>, in which the light is turned on.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>) — the number of vertices in the tree.</p><p>The second line contains <span class="tex-span"><i>n</i> - 1</span> space-separated integers <span class="tex-span"><i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> &lt; <i>i</i></span>), where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is the ancestor of vertex <span class="tex-span"><i>i</i></span>.</p><p>The third line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>), where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is <span class="tex-span">1</span>, if the light is turned on in vertex <span class="tex-span"><i>i</i></span> and <span class="tex-span">0</span> otherwise.</p><p>The fourth line contains a single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 200 000</span>) — the number of tasks.</p><p>The next <span class="tex-span"><i>q</i></span> lines are <span class="tex-font-style-tt">get v</span> or <span class="tex-font-style-tt">pow v</span> (<span class="tex-span">1 ≤ <i>v</i> ≤ <i>n</i></span>) — the tasks described above.</p>

## Output

<p>For each task <span class="tex-font-style-tt">get v</span> print the number of rooms in the subtree of <span class="tex-span"><i>v</i></span>, in which the light is turned on.</p>





```input1
4
1 1 1
1 0 0 1
9
get 1
get 2
get 3
get 4
pow 1
get 1
get 2
get 3
get 4

```




```output1
2
0
0
1
2
1
1
0

```



## Note

<center> <img class="tex-graphics" src="file://lILKRwtU.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">The tree before the task <span class="tex-font-style-tt">pow 1</span>.</span><p><img class="tex-graphics" src="file://6QGO6olz.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">The tree after the task <span class="tex-font-style-tt">pow 1</span>.</span> </p></center>
