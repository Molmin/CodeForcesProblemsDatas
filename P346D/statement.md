## Description

<div><p>The boss of the Company of Robot is a cruel man. His motto is "Move forward Or Die!". And that is exactly what his company's product do. Look at the behavior of the company's robot when it is walking in the directed graph. This behavior has been called "Three Laws of Robotics":</p><ul> <li> Law 1. The Robot will destroy itself when it visits a vertex of the graph which it has already visited. </li><li> Law 2. The Robot will destroy itself when it has no way to go (that is when it reaches a vertex whose out-degree is zero). </li><li> Law 3. The Robot will move randomly when it has multiple ways to move (that is when it reach a vertex whose out-degree is more than one). Of course, the robot can move only along the directed edges of the graph. </li></ul><p>Can you imagine a robot behaving like that? That's why they are sold at a very low price, just for those who are short of money, including mzry1992, of course. mzry1992 has such a robot, and she wants to move it from vertex <span class="tex-span"><i>s</i></span> to vertex <span class="tex-span"><i>t</i></span> in a directed graph safely without self-destruction. Luckily, she can send her robot special orders at each vertex. A special order shows the robot which way to move, if it has multiple ways to move (to prevent random moving of the robot according to Law 3). When the robot reaches vertex <span class="tex-span"><i>t</i></span>, mzry1992 takes it off the graph immediately. So you can see that, as long as there exists a path from <span class="tex-span"><i>s</i></span> to <span class="tex-span"><i>t</i></span>, she can always find a way to reach the goal (whatever the vertex <span class="tex-span"><i>t</i></span> has the outdegree of zero or not). </p><center> <img class="tex-graphics" src="file://MWwn226i.png" style="max-width: 100.0%;max-height: 100.0%;"> Sample 2 </center><p>However, sending orders is expensive, so your task is to find the minimum number of orders mzry1992 needs to send in the worst case. Please note that mzry1992 can give orders to the robot <span class="tex-font-style-bf">while it is walking</span> on the graph. Look at the first sample to clarify that part of the problem.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of vertices of the graph, and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of edges. Then <span class="tex-span"><i>m</i></span> lines follow, each with two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>; <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub> ≠ <i>u</i><sub class="lower-index"><i>i</i></sub></span>), these integers denote that there is a directed edge from vertex <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> to vertex <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. The last line contains two integers <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>s</i>, <i>t</i> ≤ <i>n</i></span>).</p><p>It is guaranteed that there are no multiple edges and self-loops.</p></div><div class="output-specification"><p>If there is a way to reach a goal, print the required minimum number of orders in the worst case. Otherwise, print -1.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of vertices of the graph, and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of edges. Then <span class="tex-span"><i>m</i></span> lines follow, each with two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>; <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub> ≠ <i>u</i><sub class="lower-index"><i>i</i></sub></span>), these integers denote that there is a directed edge from vertex <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> to vertex <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. The last line contains two integers <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>s</i>, <i>t</i> ≤ <i>n</i></span>).</p><p>It is guaranteed that there are no multiple edges and self-loops.</p>

## Output

<p>If there is a way to reach a goal, print the required minimum number of orders in the worst case. Otherwise, print -1.</p>





```input1
4 6
1 2
2 1
1 3
3 1
2 4
3 4
1 4

```




```input2
4 5
1 2
2 1
1 3
2 4
3 4
1 4

```




```output1
1

```




```output2
1

```



## Note

<p>Consider the first test sample. Initially the robot is on vertex 1. So, on the first step the robot can go to vertex 2 or 3. No matter what vertex the robot chooses, mzry1992 must give an order to the robot. This order is to go to vertex 4. If mzry1992 doesn't give an order to the robot at vertex 2 or 3, the robot can choose the "bad" outgoing edge (return to vertex 1) according Law 3. So, the answer is one.</p>
