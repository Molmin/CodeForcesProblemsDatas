## Description

<div><p>Real Cosmic Communications is the largest telecommunication company on a far far away planet, located at the very edge of the universe. RCC launches communication satellites.</p><p>The planet is at the very edge of the universe, so its form is half of a circle. Its radius is <span class="tex-span"><i>r</i></span>, the ends of its diameter are points <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span>. The line <span class="tex-span"><i>AB</i></span> is the edge of the universe, so one of the half-planes contains nothing, neither the planet, nor RCC satellites, nor anything else. Let us introduce coordinates in the following way: the origin is at the center of <span class="tex-span"><i>AB</i></span> segment, <span class="tex-span"><i>OX</i></span> axis coincides with line <span class="tex-span"><i>AB</i></span>, the planet is completely in <span class="tex-span"><i>y</i> &gt; 0</span> half-plane.</p><p>The satellite can be in any point of the universe, except the planet points. Satellites are never located beyond the edge of the universe, nor on the edge itself — that is, they have coordinate <span class="tex-span"><i>y</i> &gt; 0</span>. Satellite antennas are directed in such way that they cover the angle with the vertex in the satellite, and edges directed to points <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span>. Let us call this area the satellite <span class="tex-font-style-underline">coverage area</span>. </p><p>The picture below shows coordinate system and coverage area of a satellite.</p><center> <img class="tex-graphics" src="file://FBUtsrsR.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px"> </center><p>When RCC was founded there were no satellites around the planet. Since then there have been several events of one of the following types: </p><ol> <li> <span class="tex-font-style-tt">1 x y</span>&nbsp;— launch the new satellite and put it to the point <span class="tex-span">(<i>x</i>, <i>y</i>)</span>. Satellites never move and stay at the point they were launched. Let us assign the number <span class="tex-span"><i>i</i></span> to the <span class="tex-span"><i>i</i></span>-th satellite in order of launching, starting from one. </li><li> <span class="tex-font-style-tt">2 i</span>&nbsp;— remove satellite number <span class="tex-span"><i>i</i></span>. </li><li> <span class="tex-font-style-tt">3 i j</span>&nbsp;— make an attempt to create a communication channel between satellites <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span>. To create a communication channel a repeater is required. It must not be located inside the planet, but can be located at its half-circle border, or above it. Repeater must be in coverage area of both satellites <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span>. To avoid signal interference, it must not be located in coverage area of any other satellite. Of course, the repeater must be within the universe, it must have a coordinate <span class="tex-span"><i>y</i> &gt; 0</span>. </li></ol><p>For each attempt to create a communication channel you must find out whether it is possible.</p><p>Sample test has the following satellites locations: </p><center> <img class="tex-graphics" src="file://jN5TeaIy.png" style="max-width: 100.0%;max-height: 100.0%;" width="567px"> </center></div><div class="input-specification"><p>The first line of input data contains integers <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>n</i></span>&nbsp;— radius of the planet and the number of events (<span class="tex-span">1 ≤ <i>r</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>).</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines describe events in the specified format.</p><p>Satellite coordinates are integer, the satisfy the following constraints <span class="tex-span">|<i>x</i>| ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 &lt; <i>y</i> ≤ 10<sup class="upper-index">9</sup></span>. No two satellites that simultaneously exist can occupy the same point. Distance from each satellite to the center of the planet is strictly greater than <span class="tex-span"><i>r</i></span>.</p><p>It is guaranteed that events of types <span class="tex-span">2</span> and <span class="tex-span">3</span> only refer to satellites that exist at the moment. For all events of type <span class="tex-span">3</span> the inequality <span class="tex-span"><i>i</i> ≠ <i>j</i></span> is satisfied.</p></div><div class="output-specification"><p>For each event of type <span class="tex-span">3</span> print «<span class="tex-font-style-tt">YES</span>» on a separate line, if it is possible to create a communication channel, or «<span class="tex-font-style-tt">NO</span>» if it is impossible.</p></div>

## Input

<p>The first line of input data contains integers <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>n</i></span>&nbsp;— radius of the planet and the number of events (<span class="tex-span">1 ≤ <i>r</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>).</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines describe events in the specified format.</p><p>Satellite coordinates are integer, the satisfy the following constraints <span class="tex-span">|<i>x</i>| ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 &lt; <i>y</i> ≤ 10<sup class="upper-index">9</sup></span>. No two satellites that simultaneously exist can occupy the same point. Distance from each satellite to the center of the planet is strictly greater than <span class="tex-span"><i>r</i></span>.</p><p>It is guaranteed that events of types <span class="tex-span">2</span> and <span class="tex-span">3</span> only refer to satellites that exist at the moment. For all events of type <span class="tex-span">3</span> the inequality <span class="tex-span"><i>i</i> ≠ <i>j</i></span> is satisfied.</p>

## Output

<p>For each event of type <span class="tex-span">3</span> print «<span class="tex-font-style-tt">YES</span>» on a separate line, if it is possible to create a communication channel, or «<span class="tex-font-style-tt">NO</span>» if it is impossible.</p>





```input1
5 8
1 -5 8
1 -4 8
1 -3 8
1 2 7
3 1 3
2 2
3 1 3
3 3 4

```




```output1
NO
YES
YES

```


