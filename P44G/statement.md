## Description

<div><p>Berland amusement park shooting gallery is rightly acknowledged as one of the best in the world. Every day the country's best shooters master their skills there and the many visitors compete in clay pigeon shooting to win decent prizes. And the head of the park has recently decided to make an online version of the shooting gallery. During the elaboration process it turned out that the program that imitates the process of shooting effectively, is needed. To formulate the requirements to the program, the shooting gallery was formally described. A 3D Cartesian system of coordinates was introduced, where the <span class="tex-span"><i>X</i></span> axis ran across the gallery floor along the line, along which the shooters are located, the <span class="tex-span"><i>Y</i></span> axis ran vertically along the gallery wall and the positive direction of the <span class="tex-span"><i>Z</i></span> axis matched the shooting direction. Let's call the <span class="tex-span"><i>XOY</i></span> plane a shooting plane and let's assume that all the bullets are out of the muzzles at the points of this area and fly parallel to the <span class="tex-span"><i>Z</i></span> axis. Every clay pigeon can be represented as a rectangle whose sides are parallel to <span class="tex-span"><i>X</i></span> and <span class="tex-span"><i>Y</i></span> axes, and it has a positive <span class="tex-span"><i>z</i></span>-coordinate. The distance between a clay pigeon and the shooting plane is always different for every target. The bullet hits the target if it goes through the inner area or border of the rectangle corresponding to it. When the bullet hits the target, the target falls down vertically into the crawl-space of the shooting gallery and cannot be shot at any more. The targets are tough enough, that's why a bullet can not pierce a target all the way through and if a bullet hits a target it can't fly on. In input the simulator program is given the arrangement of all the targets and also of all the shots in the order of their appearance. The program should determine which target was hit by which shot. If you haven't guessed it yet, you are the one who is to write such a program.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of targets. Each of the subsequent <span class="tex-span"><i>n</i></span> lines contains the description of a target. The target is described by five integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>l</i></sub>, <i>x</i><sub class="lower-index"><i>r</i></sub>, <i>y</i><sub class="lower-index"><i>l</i></sub>, <i>y</i><sub class="lower-index"><i>r</i></sub>, <i>z</i></span>, that determine it's location in space (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>l</i></sub> &lt; <i>x</i><sub class="lower-index"><i>r</i></sub> ≤ 10<sup class="upper-index">7</sup>, 0 ≤ <i>y</i><sub class="lower-index"><i>l</i></sub> &lt; <i>y</i><sub class="lower-index"><i>r</i></sub> ≤ 10<sup class="upper-index">7</sup>, 0 &lt; <i>z</i> ≤ 10<sup class="upper-index">7</sup></span>). The next line contains an integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>), determining the number of shots. Then in <span class="tex-span"><i>m</i></span> lines shots are described. Every shot is determined by the coordinates of a bullet on the shooting plane <span class="tex-span">(<i>x</i>, <i>y</i>)</span> (<span class="tex-span">0 ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">7</sup></span>, the coordinates of bullets are integers). The shots are given in the order of their firing. The intervals between shots are large enough, and a target falls very quickly, that's why assume that a falling target can not be an obstruction for all the shots following the one that hit it.</p></div><div class="output-specification"><p>For every shot in the single line print the number of the target which the shot has hit, or 0, if the bullet did not hit any target. The targets are numbered starting from 1 in the order in which they were given in the input data.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of targets. Each of the subsequent <span class="tex-span"><i>n</i></span> lines contains the description of a target. The target is described by five integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>l</i></sub>, <i>x</i><sub class="lower-index"><i>r</i></sub>, <i>y</i><sub class="lower-index"><i>l</i></sub>, <i>y</i><sub class="lower-index"><i>r</i></sub>, <i>z</i></span>, that determine it's location in space (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>l</i></sub> &lt; <i>x</i><sub class="lower-index"><i>r</i></sub> ≤ 10<sup class="upper-index">7</sup>, 0 ≤ <i>y</i><sub class="lower-index"><i>l</i></sub> &lt; <i>y</i><sub class="lower-index"><i>r</i></sub> ≤ 10<sup class="upper-index">7</sup>, 0 &lt; <i>z</i> ≤ 10<sup class="upper-index">7</sup></span>). The next line contains an integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>), determining the number of shots. Then in <span class="tex-span"><i>m</i></span> lines shots are described. Every shot is determined by the coordinates of a bullet on the shooting plane <span class="tex-span">(<i>x</i>, <i>y</i>)</span> (<span class="tex-span">0 ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">7</sup></span>, the coordinates of bullets are integers). The shots are given in the order of their firing. The intervals between shots are large enough, and a target falls very quickly, that's why assume that a falling target can not be an obstruction for all the shots following the one that hit it.</p>

## Output

<p>For every shot in the single line print the number of the target which the shot has hit, or 0, if the bullet did not hit any target. The targets are numbered starting from 1 in the order in which they were given in the input data.</p>





```input1
2
1 4 1 4 1
2 5 2 6 2
4
0 0
3 3
4 5
3 5

```




```output1
0
1
2
0

```


