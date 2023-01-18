## Description

<div><p>Robot Doc is located in the hall, with <span class="tex-span"><i>n</i></span> computers stand in a line, numbered from left to right from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Each computer contains <span class="tex-font-style-bf">exactly one</span> piece of information, each of which Doc wants to get eventually. The computers are equipped with a security system, so to crack the <span class="tex-span"><i>i</i></span>-th of them, the robot needs to collect at least <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> any pieces of information from the other computers. Doc can hack the computer only if he is right next to it.</p><p>The robot is assembled using modern technologies and can move along the line of computers in either of the two possible directions, but the change of direction requires a large amount of resources from Doc. Tell the minimum number of changes of direction, which the robot will have to make to collect all <span class="tex-span"><i>n</i></span> parts of information if initially it is next to computer with number <span class="tex-span">1</span>.</p><p><span class="tex-font-style-bf">It is guaranteed</span> that there exists at least one sequence of the robot's actions, which leads to the collection of all information. Initially Doc doesn't have any pieces of information.</p></div><div class="input-specification"><p>The first line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>). The second line contains <span class="tex-span"><i>n</i></span> non-negative integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>n</i></span>), separated by a space. It is guaranteed that there exists a way for robot to collect all pieces of the information.</p></div><div class="output-specification"><p>Print a single number — the minimum number of changes in direction that the robot will have to make in order to collect all <span class="tex-span"><i>n</i></span> parts of information.</p></div>

## Input

<p>The first line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>). The second line contains <span class="tex-span"><i>n</i></span> non-negative integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>n</i></span>), separated by a space. It is guaranteed that there exists a way for robot to collect all pieces of the information.</p>

## Output

<p>Print a single number — the minimum number of changes in direction that the robot will have to make in order to collect all <span class="tex-span"><i>n</i></span> parts of information.</p>





```input1
3
0 2 0

```




```input2
5
4 2 3 0 1

```




```input3
7
0 3 1 0 5 2 6

```




```output1
1

```




```output2
3

```




```output3
2

```



## Note

<p>In the first sample you can assemble all the pieces of information in the optimal manner by assembling first the piece of information in the first computer, then in the third one, then change direction and move to the second one, and then, having 2 pieces of information, collect the last piece.</p><p>In the second sample to collect all the pieces of information in the optimal manner, Doc can go to the fourth computer and get the piece of information, then go to the fifth computer with one piece and get another one, then go to the second computer in the same manner, then to the third one and finally, to the first one. Changes of direction will take place before moving from the fifth to the second computer, then from the second to the third computer, then from the third to the first computer.</p><p>In the third sample the optimal order of collecting parts from computers can look like that: 1-&gt;3-&gt;4-&gt;6-&gt;2-&gt;5-&gt;7.</p>
