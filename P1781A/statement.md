## Description

<div><p>Vika's house has a room in a shape of a rectangular parallelepiped (also known as a rectangular cuboid). Its floor is a rectangle of size $w \times d$, and the ceiling is right above at the constant height of $h$. Let's introduce a coordinate system on the floor so that its corners are at points $(0, 0)$, $(w, 0)$, $(w, d)$, and $(0, d)$.</p><p>A laptop is standing on the floor at point $(a, b)$. A projector is hanging on the ceiling right above point $(f, g)$. Vika wants to connect the laptop and the projector with a cable in such a way that the cable always goes along the walls, ceiling, or floor (i.&nbsp;e. does not go inside the cuboid). Additionally, the cable should always run <span class="tex-font-style-bf">parallel</span> to one of the cuboid's edges (i.&nbsp;e. it can not go diagonally).</p><p>What is the minimum length of a cable that can connect the laptop to the projector?</p><center> <img class="tex-graphics" src="file://DlR9i7Bc.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px"> <span class="tex-font-size-small">Illustration for the first test case. One of the optimal ways to put the cable is shown in green.</span> </center></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains three integers $w$, $d$, and $h$ ($2 \le w, d, h \le 1000$)&nbsp;— the size of the room.</p><p>The second line contains four integers $a$, $b$, $f$, $g$ ($0 &lt; a, f &lt; w$; $0 &lt; b, g &lt; d$): the laptop is located on the floor at point $(a, b)$, while the projector is hanging on the ceiling right above point $(f, g)$.</p></div><div class="output-specification"><p>For each test case, print a single integer&nbsp;— the minimum length of the cable connecting the laptop and the projector that runs only along the walls, floor, and ceiling parallel to cuboid's edges.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains three integers $w$, $d$, and $h$ ($2 \le w, d, h \le 1000$)&nbsp;— the size of the room.</p><p>The second line contains four integers $a$, $b$, $f$, $g$ ($0 &lt; a, f &lt; w$; $0 &lt; b, g &lt; d$): the laptop is located on the floor at point $(a, b)$, while the projector is hanging on the ceiling right above point $(f, g)$.</p>

## Output

<p>For each test case, print a single integer&nbsp;— the minimum length of the cable connecting the laptop and the projector that runs only along the walls, floor, and ceiling parallel to cuboid's edges.</p>





```input1|2,3,6,7,10,11
5
55 20 29
23 10 18 3
20 10 5
1 5 2 5
15 15 4
7 13 10 10
2 1000 2
1 1 1 999
10 4 10
7 1 2 1
```




```output1
47
8
14
1002
17
```



## Note

<p>The picture in the statement illustrates the first test case.</p>
