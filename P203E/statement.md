## Description

<div><p>Valera came to Japan and bought many robots for his research. He's already at the airport, the plane will fly very soon and Valera urgently needs to bring all robots to the luggage compartment.</p><p>The robots are self-propelled (they can potentially move on their own), some of them even have compartments to carry other robots. More precisely, for the <span class="tex-span"><i>i</i></span>-th robot we know value <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> — the number of robots it can carry. In this case, each of <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> transported robots can additionally carry other robots.</p><p>However, the robots need to be filled with fuel to go, so Valera spent all his last money and bought <span class="tex-span"><i>S</i></span> liters of fuel. He learned that each robot has a restriction on travel distances. Thus, in addition to features <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, the <span class="tex-span"><i>i</i></span>-th robot has two features <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> — the amount of fuel (in liters) needed to move the <span class="tex-span"><i>i</i></span>-th robot, and the maximum distance that the robot can go.</p><p>Due to the limited amount of time and fuel, Valera wants to move the maximum number of robots to the luggage compartment. He operates as follows. </p><ul> <li> First Valera selects some robots that will travel to the luggage compartment on their own. In this case the total amount of fuel required to move all these robots must not exceed <span class="tex-span"><i>S</i></span>. </li><li> Then Valera seats the robots into the compartments, so as to transport as many robots as possible. Note that if a robot doesn't move by itself, you can put it in another not moving robot that is moved directly or indirectly by a moving robot. </li><li> After that all selected and seated robots along with Valera go to the luggage compartment and the rest robots will be lost. </li></ul><p>There are <span class="tex-span"><i>d</i></span> meters to the luggage compartment. Therefore, the robots that will carry the rest, must have feature <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> of not less than <span class="tex-span"><i>d</i></span>. During the moving Valera cannot stop or change the location of the robots in any way.</p><p>Help Valera calculate the maximum number of robots that he will be able to take home, and the minimum amount of fuel he will have to spend, because the remaining fuel will come in handy in Valera's research.</p></div><div class="input-specification"><p>The first line contains three space-separated integers <span class="tex-span"><i>n</i>, <i>d</i>, <i>S</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>d</i>, <i>S</i> ≤ 10<sup class="upper-index">9</sup>)</span>. The first number represents the number of robots, the second one — the distance to the luggage compartment and the third one — the amount of available fuel.</p><p>Next <span class="tex-span"><i>n</i></span> lines specify the robots. The <span class="tex-span"><i>i</i></span>-th line contains three space-separated integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub>, <i>f</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>f</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — the <span class="tex-span"><i>i</i></span>-th robot's features. The first number is the number of robots the <span class="tex-span"><i>i</i></span>-th robot can carry, the second number is the amount of fuel needed for the <span class="tex-span"><i>i</i></span>-th robot to move and the third one shows the maximum distance the <span class="tex-span"><i>i</i></span>-th robot can go.</p></div><div class="output-specification"><p>Print two space-separated integers — the maximum number of robots Valera can transport to the luggage compartment and the minimum amount of fuel he will need for that. If Valera won't manage to get any robots to the luggage compartment, print two zeroes.</p></div>

## Input

<p>The first line contains three space-separated integers <span class="tex-span"><i>n</i>, <i>d</i>, <i>S</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>d</i>, <i>S</i> ≤ 10<sup class="upper-index">9</sup>)</span>. The first number represents the number of robots, the second one — the distance to the luggage compartment and the third one — the amount of available fuel.</p><p>Next <span class="tex-span"><i>n</i></span> lines specify the robots. The <span class="tex-span"><i>i</i></span>-th line contains three space-separated integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub>, <i>f</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>f</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — the <span class="tex-span"><i>i</i></span>-th robot's features. The first number is the number of robots the <span class="tex-span"><i>i</i></span>-th robot can carry, the second number is the amount of fuel needed for the <span class="tex-span"><i>i</i></span>-th robot to move and the third one shows the maximum distance the <span class="tex-span"><i>i</i></span>-th robot can go.</p>

## Output

<p>Print two space-separated integers — the maximum number of robots Valera can transport to the luggage compartment and the minimum amount of fuel he will need for that. If Valera won't manage to get any robots to the luggage compartment, print two zeroes.</p>





```input1
3 10 10
0 12 10
1 6 10
0 1 1

```




```input2
2 7 10
3 12 10
5 16 8

```




```input3
4 8 10
0 12 3
1 1 0
0 3 11
1 6 9

```




```output1
2 6

```




```output2
0 0

```




```output3
4 9

```


