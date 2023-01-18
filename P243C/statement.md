## Description

<div><p>Old MacDonald has a farm and a large potato field, <span class="tex-span">(10<sup class="upper-index">10</sup> + 1) × (10<sup class="upper-index">10</sup> + 1)</span> square meters in size. The field is divided into square garden beds, each bed takes up one square meter.</p><p>Old McDonald knows that the Colorado potato beetle is about to invade his farm and can destroy the entire harvest. To fight the insects, Old McDonald wants to spray some beds with insecticides.</p><p>So Old McDonald went to the field, stood at the center of the central field bed and sprayed this bed with insecticides. Now he's going to make a series of movements and spray a few more beds. During each movement Old McDonald moves left, right, up or down the field some integer number of meters. As Old McDonald moves, he sprays all the beds he steps on. In other words, the beds that have any intersection at all with Old McDonald's trajectory, are sprayed with insecticides.</p><p>When Old McDonald finished spraying, he wrote out all his movements on a piece of paper. Now he wants to know how many beds won't be infected after the invasion of the Colorado beetles.</p><p>It is known that the invasion of the Colorado beetles goes as follows. First some bed on the field border gets infected. Than any bed that hasn't been infected, hasn't been sprayed with insecticides and has a common side with an infected bed, gets infected as well. Help Old McDonald and determine the number of beds that won't be infected by the Colorado potato beetle.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — the number of Old McDonald's movements.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain the description of Old McDonald's movements. The <span class="tex-span"><i>i</i></span>-th of these lines describes the <span class="tex-span"><i>i</i></span>-th movement. Each movement is given in the format "<span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>", where <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> is the character that determines the direction of the movement ("<span class="tex-font-style-tt">L</span>", "<span class="tex-font-style-tt">R</span>", "<span class="tex-font-style-tt">U</span>" or "<span class="tex-font-style-tt">D</span>" for directions "left", "right", "up" and "down", correspondingly), and <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) is an integer that determines the number of meters in the movement.</p></div><div class="output-specification"><p>Print a single integer — the number of beds that won't be infected by the Colorado potato beetle.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — the number of Old McDonald's movements.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain the description of Old McDonald's movements. The <span class="tex-span"><i>i</i></span>-th of these lines describes the <span class="tex-span"><i>i</i></span>-th movement. Each movement is given in the format "<span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>", where <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> is the character that determines the direction of the movement ("<span class="tex-font-style-tt">L</span>", "<span class="tex-font-style-tt">R</span>", "<span class="tex-font-style-tt">U</span>" or "<span class="tex-font-style-tt">D</span>" for directions "left", "right", "up" and "down", correspondingly), and <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) is an integer that determines the number of meters in the movement.</p>

## Output

<p>Print a single integer — the number of beds that won't be infected by the Colorado potato beetle.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
5
R 8
U 9
L 9
D 8
L 2

```




```input2
7
R 10
D 2
L 7
U 9
D 2
R 3
D 10

```




```output1
101
```




```output2
52
```


