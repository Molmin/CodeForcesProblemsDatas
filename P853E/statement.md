## Description

<div><p>After long-term research and lots of experiments leading Megapolian automobile manufacturer «AutoVoz» released a brand new car model named «Lada Malina». One of the most impressive features of «Lada Malina» is its highly efficient environment-friendly engines.</p><p>Consider car as a point in <span class="tex-span"><i>Oxy</i></span> plane. Car is equipped with <span class="tex-span"><i>k</i></span> engines numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i></span>. Each engine is defined by its velocity vector whose coordinates are <span class="tex-span">(<i>vx</i><sub class="lower-index"><i>i</i></sub>, <i>vy</i><sub class="lower-index"><i>i</i></sub>)</span> measured in distance units per day. An engine may be turned on at any level <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>, that is a real number between <span class="tex-span"> - 1</span> and <span class="tex-span"> + 1</span> (inclusive) that result in a term of <span class="tex-span">(<i>w</i><sub class="lower-index"><i>i</i></sub>·<i>vx</i><sub class="lower-index"><i>i</i></sub>, <i>w</i><sub class="lower-index"><i>i</i></sub>·<i>vy</i><sub class="lower-index"><i>i</i></sub>)</span> in the final car velocity. Namely, the final car velocity is equal to </p><center class="tex-equation"><span class="tex-span">(<i>w</i><sub class="lower-index">1</sub>·<i>vx</i><sub class="lower-index">1</sub> + <i>w</i><sub class="lower-index">2</sub>·<i>vx</i><sub class="lower-index">2</sub> + ... + <i>w</i><sub class="lower-index"><i>k</i></sub>·<i>vx</i><sub class="lower-index"><i>k</i></sub>, &nbsp;&nbsp;<i>w</i><sub class="lower-index">1</sub>·<i>vy</i><sub class="lower-index">1</sub> + <i>w</i><sub class="lower-index">2</sub>·<i>vy</i><sub class="lower-index">2</sub> + ... + <i>w</i><sub class="lower-index"><i>k</i></sub>·<i>vy</i><sub class="lower-index"><i>k</i></sub>)</span></center> <p>Formally, if car moves with constant values of <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> during the whole day then its <span class="tex-span"><i>x</i></span>-coordinate will change by the first component of an expression above, and its <span class="tex-span"><i>y</i></span>-coordinate will change by the second component of an expression above. For example, if all <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> are equal to zero, the car won't move, and if all <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> are equal to zero except <span class="tex-span"><i>w</i><sub class="lower-index">1</sub> = 1</span>, then car will move with the velocity of the first engine.</p><p>There are <span class="tex-span"><i>n</i></span> factories in Megapolia, <span class="tex-span"><i>i</i></span>-th of them is located in <span class="tex-span">(<i>fx</i><sub class="lower-index"><i>i</i></sub>, <i>fy</i><sub class="lower-index"><i>i</i></sub>)</span>. On the <span class="tex-span"><i>i</i></span>-th factory there are <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> cars «Lada Malina» that are ready for operation.</p><p>As an attempt to increase sales of a new car, «AutoVoz» is going to hold an international exposition of cars. There are <span class="tex-span"><i>q</i></span> options of exposition location and time, in the <span class="tex-span"><i>i</i></span>-th of them exposition will happen in a point with coordinates <span class="tex-span">(<i>px</i><sub class="lower-index"><i>i</i></sub>, <i>py</i><sub class="lower-index"><i>i</i></sub>)</span> in <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> days. </p><p>Of course, at the «AutoVoz» is going to bring as much new cars from factories as possible to the place of exposition. Cars are going to be moved by enabling their engines on some certain levels, such that at the beginning of an exposition car gets exactly to the exposition location. </p><p>However, for some of the options it may be impossible to bring cars from some of the factories to the exposition location by the moment of an exposition. Your task is to determine for each of the options of exposition location and time how many cars will be able to get there by the beginning of an exposition.</p></div><div class="input-specification"><p>The first line of input contains three integers <span class="tex-span"><i>k</i>, <i>n</i>, <i>q</i></span> (<span class="tex-span">2 ≤ <i>k</i> ≤ 10</span>, <span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of engines of «Lada Malina», number of factories producing «Lada Malina» and number of options of an exposition time and location respectively.</p><p>The following <span class="tex-span"><i>k</i></span> lines contain the descriptions of «Lada Malina» engines. The <span class="tex-span"><i>i</i></span>-th of them contains two integers <span class="tex-span"><i>vx</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>vy</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 1000 ≤ <i>vx</i><sub class="lower-index"><i>i</i></sub>, <i>vy</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) defining the velocity vector of the <span class="tex-span"><i>i</i></span>-th engine. Velocity vector can't be zero, i.e. at least one of <span class="tex-span"><i>vx</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>vy</i><sub class="lower-index"><i>i</i></sub></span> is not equal to zero. It is guaranteed that no two velosity vectors are collinear (parallel).</p><p>Next <span class="tex-span"><i>n</i></span> lines contain the descriptions of factories. The <span class="tex-span"><i>i</i></span>-th of them contains two integers <span class="tex-span"><i>fx</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>fy</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>fx</i><sub class="lower-index"><i>i</i></sub>, <i>fy</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) defining the coordinates of the <span class="tex-span"><i>i</i></span>-th factory location and the number of cars that are located there.</p><p>The following <span class="tex-span"><i>q</i></span> lines contain the descriptions of the car exposition. The <span class="tex-span"><i>i</i></span>-th of them contains three integers <span class="tex-span"><i>px</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>py</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>px</i><sub class="lower-index"><i>i</i></sub>, <i>py</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>) defining the coordinates of the exposition location and the number of days till the exposition start in the <span class="tex-span"><i>i</i></span>-th option.</p></div><div class="output-specification"><p>For each possible option of the exposition output the number of cars that will be able to get to the exposition location by the moment of its beginning.</p></div>

## Input

<p>The first line of input contains three integers <span class="tex-span"><i>k</i>, <i>n</i>, <i>q</i></span> (<span class="tex-span">2 ≤ <i>k</i> ≤ 10</span>, <span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of engines of «Lada Malina», number of factories producing «Lada Malina» and number of options of an exposition time and location respectively.</p><p>The following <span class="tex-span"><i>k</i></span> lines contain the descriptions of «Lada Malina» engines. The <span class="tex-span"><i>i</i></span>-th of them contains two integers <span class="tex-span"><i>vx</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>vy</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 1000 ≤ <i>vx</i><sub class="lower-index"><i>i</i></sub>, <i>vy</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) defining the velocity vector of the <span class="tex-span"><i>i</i></span>-th engine. Velocity vector can't be zero, i.e. at least one of <span class="tex-span"><i>vx</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>vy</i><sub class="lower-index"><i>i</i></sub></span> is not equal to zero. It is guaranteed that no two velosity vectors are collinear (parallel).</p><p>Next <span class="tex-span"><i>n</i></span> lines contain the descriptions of factories. The <span class="tex-span"><i>i</i></span>-th of them contains two integers <span class="tex-span"><i>fx</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>fy</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>fx</i><sub class="lower-index"><i>i</i></sub>, <i>fy</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) defining the coordinates of the <span class="tex-span"><i>i</i></span>-th factory location and the number of cars that are located there.</p><p>The following <span class="tex-span"><i>q</i></span> lines contain the descriptions of the car exposition. The <span class="tex-span"><i>i</i></span>-th of them contains three integers <span class="tex-span"><i>px</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>py</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>px</i><sub class="lower-index"><i>i</i></sub>, <i>py</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>) defining the coordinates of the exposition location and the number of days till the exposition start in the <span class="tex-span"><i>i</i></span>-th option.</p>

## Output

<p>For each possible option of the exposition output the number of cars that will be able to get to the exposition location by the moment of its beginning.</p>





```input1
2 4 1
1 1
-1 1
2 3 1
2 -2 1
-2 1 1
-2 -2 1
0 0 2

```




```input2
3 4 3
2 0
-1 1
-1 -2
-3 0 6
1 -2 1
-3 -7 3
3 2 2
-1 -4 1
0 4 2
6 0 1

```




```output1
3

```




```output2
4
9
0

```



## Note

<p>Images describing sample tests are given below. Exposition options are denoted with crosses, factories are denoted with points. Each factory is labeled with a number of cars that it has.</p><p>First sample test explanation:</p><ul> <li> Car from the first factory is not able to get to the exposition location in time. </li><li> Car from the second factory can get to the exposition in time if we set <span class="tex-span"><i>w</i><sub class="lower-index">1</sub> = 0</span>, <span class="tex-span"><i>w</i><sub class="lower-index">2</sub> = 1</span>. </li><li> Car from the third factory can get to the exposition in time if we set <img align="middle" class="tex-formula" src="file://NWFrigfp.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://13NOKpdf.png" style="max-width: 100.0%;max-height: 100.0%;">. </li><li> Car from the fourth factory can get to the exposition in time if we set <span class="tex-span"><i>w</i><sub class="lower-index">1</sub> = 1</span>, <span class="tex-span"><i>w</i><sub class="lower-index">2</sub> = 0</span>. </li></ul><center> <img class="tex-graphics" src="file://e9NfogAI.png" style="max-width: 100.0%;max-height: 100.0%;" width="302px"> <img class="tex-graphics" src="file://OXFh4mNn.png" style="max-width: 100.0%;max-height: 100.0%;" width="302px"> </center>
