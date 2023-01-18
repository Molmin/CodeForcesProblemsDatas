## Description

<div><p>The first ship with the Earth settlers landed on Mars. The colonists managed to build <span class="tex-span"><i>n</i></span> necessary structures on the surface of the planet (which can be regarded as a plane, and the construction can be regarded as points on it). But one day the scanners recorded suspicious activity on the outskirts of the colony. It was decided to use the protective force field generating system to protect the colony against possible trouble.</p><p>The system works as follows: the surface contains a number of generators of the field (they can also be considered as points). The active range of each generator is a circle of radius <span class="tex-span"><i>r</i></span> centered at the location of the generator (the boundary of the circle is also included in the range). After the system is activated, it stretches the protective force field <span class="tex-font-style-bf">only over the part of the surface, which is within the area of all generators' activity</span>. That is, the protected part is the <span class="tex-font-style-bf">intersection</span> of the generators' active ranges.</p><p>The number of generators available to the colonists is not limited, but the system of field generation consumes a lot of energy. More precisely, the energy consumption does not depend on the number of generators, but it is directly proportional to the <span class="tex-font-style-bf">area</span>, which is protected by the field. Also, it is necessary that all the existing buildings are located within the protected area.</p><p>Determine the smallest possible area of the protected part of the surface containing all the buildings.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>r</i> ≤ 50000</span>) — the number of buildings and the active ranges of the generators, correspondingly.</p><p>Next <span class="tex-span"><i>n</i></span> lines contains the buildings' coordinates. The <span class="tex-span"><i>i</i> + 1</span>-th (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) line contains two real numbers with at most three digits after the decimal point <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 50000</span>) — coordinates of the <span class="tex-span"><i>i</i></span>-th building. It is guaranteed that no two buildings are located at the same point, and no two different buildings are located closer than <span class="tex-span">1</span>.</p><p>It is guaranteed that there exists a circle with radius <span class="tex-span"><i>r</i></span> that contains all the buildings.</p></div><div class="output-specification"><p>Print the single real number — the minimum area of the protected part containing all the buildings. The answer is accepted if absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>r</i> ≤ 50000</span>) — the number of buildings and the active ranges of the generators, correspondingly.</p><p>Next <span class="tex-span"><i>n</i></span> lines contains the buildings' coordinates. The <span class="tex-span"><i>i</i> + 1</span>-th (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) line contains two real numbers with at most three digits after the decimal point <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 50000</span>) — coordinates of the <span class="tex-span"><i>i</i></span>-th building. It is guaranteed that no two buildings are located at the same point, and no two different buildings are located closer than <span class="tex-span">1</span>.</p><p>It is guaranteed that there exists a circle with radius <span class="tex-span"><i>r</i></span> that contains all the buildings.</p>

## Output

<p>Print the single real number — the minimum area of the protected part containing all the buildings. The answer is accepted if absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p>





```input1
3 5
0.00 0.000
0.0 8.00
6 8.00

```




```input2
4 1000
0.0 0.0
0 2.00
2.00 2
2.0 0.00

```




```input3
4 5
3.00 0.0
-3 0.00
0.000 1
0.0 -1.00

```




```output1
78.5398163397

```




```output2
4.0026666140

```




```output3
8.1750554397

```



## Note

<p>In the first sample the given radius equals the radius of the circle circumscribed around the given points. That's why the circle that corresponds to it is the sought area. The answer is <span class="tex-span">25π</span>.</p><p>In the second sample the area nearly coincides with the square which has vertexes in the given points.</p><p>The area for the third sample is shown on the picture below.</p><center> <img class="tex-graphics" src="file://sV5oV2EF.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
