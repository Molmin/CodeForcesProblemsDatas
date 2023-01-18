## Description

<div><p>Don't put up with what you're sick of! The Smart Beaver decided to escape from the campus of Beaver Science Academy (BSA). BSA is a <span class="tex-span"><i>b</i> × <i>b</i></span> square on a plane. Each point <span class="tex-span"><i>x</i>, <i>y</i></span> <span class="tex-span">(0 ≤ <i>x</i>, <i>y</i> ≤ <i>b</i>)</span> belongs to BSA. To make the path quick and funny, the Beaver constructed a Beaveractor, an effective and comfortable types of transport.</p><p>The campus obeys traffic rules: there are <span class="tex-span"><i>n</i></span> arrows, parallel to the coordinate axes. The arrows do not intersect and do not touch each other. When the Beaveractor reaches some arrow, it turns in the arrow's direction and moves on until it either reaches the next arrow or gets outside the campus. The Beaveractor covers exactly one unit of space per one unit of time. You can assume that there are no obstacles to the Beaveractor.</p><p>The BSA scientists want to transport the brand new Beaveractor to the "Academic Tractor" research institute and send the Smart Beaver to do his postgraduate studies and sharpen pencils. They have <span class="tex-span"><i>q</i></span> plans, representing the Beaveractor's initial position <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>, the initial motion vector <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> and the time <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> that have passed after the escape started.</p><p>Your task is for each of the <span class="tex-span"><i>q</i></span> plans to determine the Smart Beaver's position after the given time.</p></div><div class="input-specification"><p>The first line contains two integers: the number of traffic rules <span class="tex-span"><i>n</i></span> and the size of the campus <span class="tex-span"><i>b</i></span>, <span class="tex-span">0 ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>b</i></span>. Next <span class="tex-span"><i>n</i></span> lines contain the rules. Each line of the rules contains four space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index">0</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">0</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span> — the beginning and the end of the arrow. It is guaranteed that all arrows are parallel to the coordinate axes and have no common points. All arrows are located inside the campus, that is, <span class="tex-span">0 ≤ <i>x</i><sub class="lower-index">0</sub>, <i>y</i><sub class="lower-index">0</sub>, <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub> ≤ <i>b</i></span> holds.</p><p>Next line contains integer <span class="tex-span"><i>q</i></span> — the number of plans the scientists have, <span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>. The <span class="tex-span"><i>i</i></span>-th plan is represented by two integers, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> are the Beaveractor's coordinates at the initial time, <span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>b</i></span>, character <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>, that takes value <span class="tex-font-style-tt">U</span>, <span class="tex-font-style-tt">D</span>, <span class="tex-font-style-tt">L</span>, <span class="tex-font-style-tt">R</span> and sets the initial direction up, down, to the left or to the right correspondingly (the Y axis is directed upwards), and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> — the time passed after the escape started, <span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">15</sup></span>.</p><ul> <li> to get 30 points you need to solve the problem with constraints <span class="tex-span"><i>n</i>, <i>b</i> ≤ 30</span> (subproblem D1); </li><li> to get 60 points you need to solve the problem with constraints <span class="tex-span"><i>n</i>, <i>b</i> ≤ 1000</span> (subproblems D1+D2); </li><li> to get 100 points you need to solve the problem with constraints <span class="tex-span"><i>n</i>, <i>b</i> ≤ 10<sup class="upper-index">5</sup></span> (subproblems D1+D2+D3). </li></ul></div><div class="output-specification"><p>Print <span class="tex-span"><i>q</i></span> lines. Each line should contain two integers — the Beaveractor's coordinates at the final moment of time for each plan. If the Smart Beaver manages to leave the campus in time <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, print the coordinates of the last point in the campus he visited.</p></div>

## Input

<p>The first line contains two integers: the number of traffic rules <span class="tex-span"><i>n</i></span> and the size of the campus <span class="tex-span"><i>b</i></span>, <span class="tex-span">0 ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>b</i></span>. Next <span class="tex-span"><i>n</i></span> lines contain the rules. Each line of the rules contains four space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index">0</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">0</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span> — the beginning and the end of the arrow. It is guaranteed that all arrows are parallel to the coordinate axes and have no common points. All arrows are located inside the campus, that is, <span class="tex-span">0 ≤ <i>x</i><sub class="lower-index">0</sub>, <i>y</i><sub class="lower-index">0</sub>, <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub> ≤ <i>b</i></span> holds.</p><p>Next line contains integer <span class="tex-span"><i>q</i></span> — the number of plans the scientists have, <span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>. The <span class="tex-span"><i>i</i></span>-th plan is represented by two integers, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> are the Beaveractor's coordinates at the initial time, <span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>b</i></span>, character <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>, that takes value <span class="tex-font-style-tt">U</span>, <span class="tex-font-style-tt">D</span>, <span class="tex-font-style-tt">L</span>, <span class="tex-font-style-tt">R</span> and sets the initial direction up, down, to the left or to the right correspondingly (the Y axis is directed upwards), and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> — the time passed after the escape started, <span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">15</sup></span>.</p><ul> <li> to get 30 points you need to solve the problem with constraints <span class="tex-span"><i>n</i>, <i>b</i> ≤ 30</span> (subproblem D1); </li><li> to get 60 points you need to solve the problem with constraints <span class="tex-span"><i>n</i>, <i>b</i> ≤ 1000</span> (subproblems D1+D2); </li><li> to get 100 points you need to solve the problem with constraints <span class="tex-span"><i>n</i>, <i>b</i> ≤ 10<sup class="upper-index">5</sup></span> (subproblems D1+D2+D3). </li></ul>

## Output

<p>Print <span class="tex-span"><i>q</i></span> lines. Each line should contain two integers — the Beaveractor's coordinates at the final moment of time for each plan. If the Smart Beaver manages to leave the campus in time <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, print the coordinates of the last point in the campus he visited.</p>





```input1
3 3
0 0 0 1
0 2 2 2
3 3 2 3
12
0 0 L 0
0 0 L 1
0 0 L 2
0 0 L 3
0 0 L 4
0 0 L 5
0 0 L 6
2 0 U 2
2 0 U 3
3 0 U 5
1 3 D 2
1 3 R 2

```




```output1
0 0
0 1
0 2
1 2
2 2
3 2
3 2
2 2
3 2
1 3
2 2
1 3

```


