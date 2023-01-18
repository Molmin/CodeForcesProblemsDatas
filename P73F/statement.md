## Description

<div><p>Vasya plays the Plane of Tanks. The tanks in this game keep trying to finish each other off. But your "Pedalny" is not like that... He just needs to drive in a straight line from point <span class="tex-span"><i>A</i></span> to point B on the plane. Unfortunately, on the same plane are <span class="tex-span"><i>n</i></span> enemy tanks. We shall regard all the tanks as points. At the initial moment of time Pedalny is at the point <span class="tex-span"><i>A</i></span>. Enemy tanks would be happy to destroy it immediately, but initially their turrets are tuned in other directions. Specifically, for each tank we know the initial rotation of the turret <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (the angle in radians relative to the <span class="tex-span"><i>OX</i></span> axis in the counterclockwise direction) and the maximum speed of rotation of the turret <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (radians per second). If at any point of time a tank turret will be aimed precisely at the tank Pedalny, then the enemy fires and it never misses. Pedalny can endure no more than <span class="tex-span"><i>k</i></span> shots. Gun reloading takes very much time, so we can assume that every enemy will produce no more than one shot. Your task is to determine what minimum speed of <span class="tex-span"><i>v</i></span> Pedalny must have to get to the point <span class="tex-span"><i>B</i></span>. It is believed that Pedalny is able to instantly develop the speed of <span class="tex-span"><i>v</i></span>, and the first <span class="tex-span"><i>k</i></span> shots at him do not reduce the speed and do not change the coordinates of the tank.</p></div><div class="input-specification"><p>The first line contains 4 numbers – the coordinates of points <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> (in meters), the points do not coincide. On the second line number <span class="tex-span"><i>n</i></span> is given (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup></span>). It is the number of enemy tanks. Each of the following <span class="tex-span"><i>n</i></span> lines contain the coordinates of a corresponding tank <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> and its parameters <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 2π</span>, <span class="tex-span">0 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>). Numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> contain at most 5 digits after the decimal point. All coordinates are integers and their absolute values do not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>. Enemy tanks can rotate a turret in the clockwise as well as in the counterclockwise direction at the angular speed of not more than <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>. It is guaranteed that each of the enemy tanks will need at least <span class="tex-span">0.1</span> seconds to aim at any point of the segment <span class="tex-span"><i>AB</i></span> and each of the enemy tanks is posistioned no closer than <span class="tex-span">0.1</span> meters to line <span class="tex-span"><i>AB</i></span>. On the last line is given the number <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ <i>n</i></span>).</p></div><div class="output-specification"><p>Print a single number with absolute or relative error no more than <span class="tex-span">10<sup class="upper-index"> - 4</sup></span> — the minimum required speed of Pedalny in meters per second.</p></div>

## Input

<p>The first line contains 4 numbers – the coordinates of points <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> (in meters), the points do not coincide. On the second line number <span class="tex-span"><i>n</i></span> is given (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup></span>). It is the number of enemy tanks. Each of the following <span class="tex-span"><i>n</i></span> lines contain the coordinates of a corresponding tank <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> and its parameters <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 2π</span>, <span class="tex-span">0 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>). Numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> contain at most 5 digits after the decimal point. All coordinates are integers and their absolute values do not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>. Enemy tanks can rotate a turret in the clockwise as well as in the counterclockwise direction at the angular speed of not more than <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>. It is guaranteed that each of the enemy tanks will need at least <span class="tex-span">0.1</span> seconds to aim at any point of the segment <span class="tex-span"><i>AB</i></span> and each of the enemy tanks is posistioned no closer than <span class="tex-span">0.1</span> meters to line <span class="tex-span"><i>AB</i></span>. On the last line is given the number <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ <i>n</i></span>).</p>

## Output

<p>Print a single number with absolute or relative error no more than <span class="tex-span">10<sup class="upper-index"> - 4</sup></span> — the minimum required speed of Pedalny in meters per second.</p>





```input1
0 0 10 0
1
5 -5 4.71238 1
0

```




```input2
0 0 10 0
1
5 -5 4.71238 1
1

```




```output1
4.2441

```




```output2
0.0000

```


