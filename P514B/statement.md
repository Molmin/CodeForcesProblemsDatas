## Description

<div><p>There are <span class="tex-span"><i>n</i></span> Imperial stormtroopers on the field. The battle field is a plane with Cartesian coordinate system. Each stormtrooper is associated with his coordinates <span class="tex-span">(<i>x</i>, <i>y</i>)</span> on this plane. </p><p>Han Solo has the newest duplex lazer gun to fight these stormtroopers. It is situated at the point <span class="tex-span">(<i>x</i><sub class="lower-index">0</sub>, <i>y</i><sub class="lower-index">0</sub>)</span>. In one shot it can can destroy all the stormtroopers, situated on some line that crosses point <span class="tex-span">(<i>x</i><sub class="lower-index">0</sub>, <i>y</i><sub class="lower-index">0</sub>)</span>.</p><p>Your task is to determine what minimum number of shots Han Solo needs to defeat all the stormtroopers.</p><p>The gun is the newest invention, it shoots very quickly and even after a very large number of shots the stormtroopers don't have enough time to realize what's happening and change their location. </p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index">0</sub></span> и <span class="tex-span"><i>y</i><sub class="lower-index">0</sub></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span"> - 10<sup class="upper-index">4</sup> ≤ <i>x</i><sub class="lower-index">0</sub>, <i>y</i><sub class="lower-index">0</sub> ≤ 10<sup class="upper-index">4</sup></span>) — the number of stormtroopers on the battle field and the coordinates of your gun.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain two integers each <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">4</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>) — the coordinates of the stormtroopers on the battlefield. It is guaranteed that no stormtrooper stands at the same point with the gun. Multiple stormtroopers can stand at the same point.</p></div><div class="output-specification"><p>Print a single integer — the minimum number of shots Han Solo needs to destroy all the stormtroopers. </p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index">0</sub></span> и <span class="tex-span"><i>y</i><sub class="lower-index">0</sub></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span"> - 10<sup class="upper-index">4</sup> ≤ <i>x</i><sub class="lower-index">0</sub>, <i>y</i><sub class="lower-index">0</sub> ≤ 10<sup class="upper-index">4</sup></span>) — the number of stormtroopers on the battle field and the coordinates of your gun.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain two integers each <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">4</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>) — the coordinates of the stormtroopers on the battlefield. It is guaranteed that no stormtrooper stands at the same point with the gun. Multiple stormtroopers can stand at the same point.</p>

## Output

<p>Print a single integer — the minimum number of shots Han Solo needs to destroy all the stormtroopers. </p>





```input1
4 0 0
1 1
2 2
2 0
-1 -1

```




```input2
2 1 2
1 1
1 0

```




```output1
2

```




```output2
1

```



## Note

<p>Explanation to the first and second samples from the statement, respectively: </p><center> <img class="tex-graphics" src="file://jAk3Bk4f.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
