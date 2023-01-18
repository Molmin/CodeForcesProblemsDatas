## Description

<div><p>Girl Lena likes it when everything is in order, and looks for order everywhere. Once she was getting ready for the University and noticed that the room was in a mess — all the objects from her handbag were thrown about the room. Of course, she wanted to put them back into her handbag. The problem is that the girl cannot carry more than two objects at a time, and cannot move the handbag. Also, if he has taken an object, she cannot put it anywhere except her handbag — her inherent sense of order does not let her do so.</p><p>You are given the coordinates of the handbag and the coordinates of the objects in some Сartesian coordinate system. It is known that the girl covers the distance between any two objects in the time equal to the squared length of the segment between the points of the objects. It is also known that initially the coordinates of the girl and the handbag are the same. You are asked to find such an order of actions, that the girl can put all the objects back into her handbag in a minimum time period.</p></div><div class="input-specification"><p>The first line of the input file contains the handbag's coordinates <span class="tex-span"><i>x</i><sub class="lower-index"><i>s</i></sub>, <i>y</i><sub class="lower-index"><i>s</i></sub></span>. The second line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 24</span>) — the amount of objects the girl has. The following <span class="tex-span"><i>n</i></span> lines contain the objects' coordinates. All the coordinates do not exceed 100 in absolute value. All the given positions are different. All the numbers are integer.</p></div><div class="output-specification"><p>In the first line output the only number — the minimum time the girl needs to put the objects into her handbag. </p><p>In the second line output the possible optimum way for Lena. Each object in the input is described by its index number (from 1 to <span class="tex-span"><i>n</i></span>), the handbag's point is described by number 0. The path should start and end in the handbag's point. If there are several optimal paths, print any of them. </p></div>

## Input

<p>The first line of the input file contains the handbag's coordinates <span class="tex-span"><i>x</i><sub class="lower-index"><i>s</i></sub>, <i>y</i><sub class="lower-index"><i>s</i></sub></span>. The second line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 24</span>) — the amount of objects the girl has. The following <span class="tex-span"><i>n</i></span> lines contain the objects' coordinates. All the coordinates do not exceed 100 in absolute value. All the given positions are different. All the numbers are integer.</p>

## Output

<p>In the first line output the only number — the minimum time the girl needs to put the objects into her handbag. </p><p>In the second line output the possible optimum way for Lena. Each object in the input is described by its index number (from 1 to <span class="tex-span"><i>n</i></span>), the handbag's point is described by number 0. The path should start and end in the handbag's point. If there are several optimal paths, print any of them. </p>





```input1
0 0
2
1 1
-1 1

```




```input2
1 1
3
4 3
3 4
0 0

```




```output1
8
0 1 2 0 

```




```output2
32
0 1 2 0 3 0 

```


