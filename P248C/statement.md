## Description

<div><p>It's a beautiful April day and Wallace is playing football with his friends. But his friends do not know that Wallace actually stayed home with Gromit and sent them his robotic self instead. Robo-Wallace has several advantages over the other guys. For example, he can hit the ball directly to the specified point. And yet, the notion of a giveaway is foreign to him. The combination of these features makes the Robo-Wallace the perfect footballer — as soon as the ball gets to him, he can just aim and hit the goal. He followed this tactics in the first half of the match, but he hit the goal rarely. The opposing team has a very good goalkeeper who catches most of the balls that fly directly into the goal. But Robo-Wallace is a quick thinker, he realized that he can cheat the goalkeeper. After all, they are playing in a football box with solid walls. Robo-Wallace can kick the ball to the other side, then the goalkeeper will not try to catch the ball. Then, if the ball bounces off the wall and flies into the goal, the goal will at last be scored.</p><p>Your task is to help Robo-Wallace to detect a spot on the wall of the football box, to which the robot should kick the ball, so that the ball bounces once and only once off this wall and goes straight to the goal. In the first half of the match Robo-Wallace got a ball in the head and was severely hit. As a result, some of the schemes have been damaged. Because of the damage, Robo-Wallace can only aim to his right wall (Robo-Wallace is standing with his face to the opposing team's goal).</p><p>The football box is rectangular. Let's introduce a two-dimensional coordinate system so that point (<span class="tex-span">0</span>, <span class="tex-span">0</span>) lies in the lower left corner of the field, if you look at the box above. Robo-Wallace is playing for the team, whose goal is to the right. It is an improvised football field, so the gate of Robo-Wallace's rivals may be not in the middle of the left wall.</p><center> <img class="tex-graphics" src="file://4FPZVeOR.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the given coordinate system you are given: </p><ul> <li> <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> — the <span class="tex-span"><i>y</i></span>-coordinates of the side pillars of the goalposts of robo-Wallace's opponents; </li><li> <span class="tex-span"><i>y</i><sub class="lower-index"><i>w</i></sub></span> — the <span class="tex-span"><i>y</i></span>-coordinate of the wall to which Robo-Wallace is aiming; </li><li> <span class="tex-span"><i>x</i><sub class="lower-index"><i>b</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>b</i></sub></span> — the coordinates of the ball's position when it is hit; </li><li> <span class="tex-span"><i>r</i></span> — the radius of the ball. </li></ul><p>A goal is scored when the center of the ball crosses the <span class="tex-span"><i>OY</i></span> axis in the given coordinate system between (<span class="tex-span">0</span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>) and (<span class="tex-span">0</span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span>). The ball moves along a straight line. The ball's hit on the wall is perfectly elastic (the ball does not shrink from the hit), the angle of incidence equals the angle of reflection. If the ball bounces off the wall not to the goal, that is, if it hits the other wall or the goal post, then the opposing team catches the ball and Robo-Wallace starts looking for miscalculation and gets dysfunctional. Such an outcome, if possible, should be avoided. We assume that the ball touches an object, if the distance from the center of the ball to the object is no greater than the ball radius <span class="tex-span"><i>r</i></span>.</p></div><div class="input-specification"><p>The first and the single line contains integers <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>w</i></sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>b</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>b</i></sub></span>, <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index"><i>w</i></sub>, <i>x</i><sub class="lower-index"><i>b</i></sub>, <i>y</i><sub class="lower-index"><i>b</i></sub> ≤ 10<sup class="upper-index">6</sup></span>; <span class="tex-span"><i>y</i><sub class="lower-index">1</sub> &lt; <i>y</i><sub class="lower-index">2</sub> &lt; <i>y</i><sub class="lower-index"><i>w</i></sub></span>; <span class="tex-span"><i>y</i><sub class="lower-index"><i>b</i></sub> + <i>r</i> &lt; <i>y</i><sub class="lower-index"><i>w</i></sub></span>; <span class="tex-span">2·<i>r</i> &lt; <i>y</i><sub class="lower-index">2</sub> - <i>y</i><sub class="lower-index">1</sub></span>).</p><p>It is guaranteed that the ball is positioned correctly in the field, doesn't cross any wall, doesn't touch the wall that Robo-Wallace is aiming at. The goal posts can't be located in the field corners.</p></div><div class="output-specification"><p>If Robo-Wallace can't score a goal in the described manner, print "-1" (without the quotes). Otherwise, print a single number <span class="tex-span"><i>x</i><sub class="lower-index"><i>w</i></sub></span> — the abscissa of his point of aiming. </p><p>If there are multiple points of aiming, print the abscissa of any of them. When checking the correctness of the answer, all comparisons are made with the permissible absolute error, equal to <span class="tex-span">10<sup class="upper-index"> - 8</sup></span>. </p><p>It is recommended to print as many characters after the decimal point as possible.</p></div>

## Input

<p>The first and the single line contains integers <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>w</i></sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>b</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>b</i></sub></span>, <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index"><i>w</i></sub>, <i>x</i><sub class="lower-index"><i>b</i></sub>, <i>y</i><sub class="lower-index"><i>b</i></sub> ≤ 10<sup class="upper-index">6</sup></span>; <span class="tex-span"><i>y</i><sub class="lower-index">1</sub> &lt; <i>y</i><sub class="lower-index">2</sub> &lt; <i>y</i><sub class="lower-index"><i>w</i></sub></span>; <span class="tex-span"><i>y</i><sub class="lower-index"><i>b</i></sub> + <i>r</i> &lt; <i>y</i><sub class="lower-index"><i>w</i></sub></span>; <span class="tex-span">2·<i>r</i> &lt; <i>y</i><sub class="lower-index">2</sub> - <i>y</i><sub class="lower-index">1</sub></span>).</p><p>It is guaranteed that the ball is positioned correctly in the field, doesn't cross any wall, doesn't touch the wall that Robo-Wallace is aiming at. The goal posts can't be located in the field corners.</p>

## Output

<p>If Robo-Wallace can't score a goal in the described manner, print "-1" (without the quotes). Otherwise, print a single number <span class="tex-span"><i>x</i><sub class="lower-index"><i>w</i></sub></span> — the abscissa of his point of aiming. </p><p>If there are multiple points of aiming, print the abscissa of any of them. When checking the correctness of the answer, all comparisons are made with the permissible absolute error, equal to <span class="tex-span">10<sup class="upper-index"> - 8</sup></span>. </p><p>It is recommended to print as many characters after the decimal point as possible.</p>





```input1
4 10 13 10 3 1

```




```input2
1 4 6 2 2 1

```




```input3
3 10 15 17 9 2

```




```output1
4.3750000000

```




```output2
-1

```




```output3
11.3333333333

```



## Note

<p>Note that in the first and third samples other correct values of abscissa <span class="tex-span"><i>x</i><sub class="lower-index"><i>w</i></sub></span> are also possible.</p>
