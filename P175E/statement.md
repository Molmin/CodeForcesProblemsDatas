## Description

<div><p>Vasya plays the Power Defence. </p><p>He must pass the last level of the game. In order to do this he must kill the Main Villain, who moves in a straight line at speed 1 meter per second from the point <span class="tex-span">( - ∞, 0)</span> to the point <span class="tex-span">( + ∞, 0)</span> of the game world. In the points <span class="tex-span">(<i>x</i>, 1)</span> and <span class="tex-span">(<i>x</i>,  - 1)</span>, where <span class="tex-span"><i>x</i></span> is an integer number, Vasya can build towers of three types: fire-tower, electric-tower or freezing-tower. However, it is not allowed to build two towers at the same point. Towers of each type have a certain action radius and the value of damage per second (except freezing-tower). If at some point the Main Villain is in the range of action of <span class="tex-span"><i>k</i></span> freezing towers then his speed is decreased by <span class="tex-span"><i>k</i> + 1</span> times.</p><p>The allowed number of towers of each type is known. It is necessary to determine the maximum possible damage we can inflict on the Main Villain.</p><p>All distances in the problem are given in meters. The size of the Main Villain and the towers are so small, that they can be considered as points on the plane. The Main Villain is in the action radius of a tower if the distance between him and tower is less than or equal to the action radius of the tower.</p></div><div class="input-specification"><p>The first line contains three integer numbers <span class="tex-span"><i>nf</i>, <i>ne</i></span> and <span class="tex-span"><i>ns</i></span> — the maximum number of fire-towers, electric-towers and freezing-towers that can be built <span class="tex-span">(0 ≤ <i>nf</i>, <i>ne</i>, <i>ns</i> ≤ 20, 1 ≤ <i>nf</i> + <i>ne</i> + <i>ns</i> ≤ 20)</span>. The numbers are separated with single spaces.</p><p>The second line contains three integer numbers <span class="tex-span"><i>rf</i>, <i>re</i></span> and <span class="tex-span"><i>rs</i></span> <span class="tex-span">(1 ≤ <i>rf</i>, <i>re</i>, <i>rs</i> ≤ 1000)</span> — the action radii of fire-towers, electric-towers and freezing-towers. The numbers are separated with single spaces.</p><p>The third line contains two integer numbers <span class="tex-span"><i>df</i></span> and <span class="tex-span"><i>de</i></span> <span class="tex-span">(1 ≤ <i>df</i>, <i>de</i> ≤ 1000)</span> — the damage a fire-tower and an electronic-tower can inflict on the Main Villain per second (in the case when the Main Villain is in the action radius of the tower). The numbers are separated with single space.</p></div><div class="output-specification"><p>Print the only real number — the maximum possible damage to the Main Villain with absolute or relative error not more than <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line contains three integer numbers <span class="tex-span"><i>nf</i>, <i>ne</i></span> and <span class="tex-span"><i>ns</i></span> — the maximum number of fire-towers, electric-towers and freezing-towers that can be built <span class="tex-span">(0 ≤ <i>nf</i>, <i>ne</i>, <i>ns</i> ≤ 20, 1 ≤ <i>nf</i> + <i>ne</i> + <i>ns</i> ≤ 20)</span>. The numbers are separated with single spaces.</p><p>The second line contains three integer numbers <span class="tex-span"><i>rf</i>, <i>re</i></span> and <span class="tex-span"><i>rs</i></span> <span class="tex-span">(1 ≤ <i>rf</i>, <i>re</i>, <i>rs</i> ≤ 1000)</span> — the action radii of fire-towers, electric-towers and freezing-towers. The numbers are separated with single spaces.</p><p>The third line contains two integer numbers <span class="tex-span"><i>df</i></span> and <span class="tex-span"><i>de</i></span> <span class="tex-span">(1 ≤ <i>df</i>, <i>de</i> ≤ 1000)</span> — the damage a fire-tower and an electronic-tower can inflict on the Main Villain per second (in the case when the Main Villain is in the action radius of the tower). The numbers are separated with single space.</p>

## Output

<p>Print the only real number — the maximum possible damage to the Main Villain with absolute or relative error not more than <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
1 0 0
10 10 10
100 100

```




```input2
1 0 1
10 10 10
100 100

```




```output1
1989.97487421
```




```output2
3979.94974843
```



## Note

<p>In the first sample we've got one fire-tower that always inflicts the same damage, independently of its position. </p><p>In the second sample we've got another freezing-tower of the same action radius. If we build the two towers opposite each other, then the Main Villain's speed will be two times lower, whenever he enters the fire-tower's action radius. That means that the enemy will be inflicted with twice more damage.</p>
