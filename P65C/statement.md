## Description

<div><p>Brothers Fred and George Weasley once got into the sporting goods store and opened a box of Quidditch balls. After long and painful experiments they found out that the Golden Snitch is not enchanted at all. It is simply a programmed device. It always moves along the same trajectory, which is a polyline with vertices at the points <span class="tex-span">(<i>x</i><sub class="lower-index">0</sub>, <i>y</i><sub class="lower-index">0</sub>, <i>z</i><sub class="lower-index">0</sub>)</span>, <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>z</i><sub class="lower-index">1</sub>)</span>, ..., <span class="tex-span">(<i>x</i><sub class="lower-index"><i>n</i></sub>, <i>y</i><sub class="lower-index"><i>n</i></sub>, <i>z</i><sub class="lower-index"><i>n</i></sub>)</span>. At the beginning of the game the snitch is positioned at the point <span class="tex-span">(<i>x</i><sub class="lower-index">0</sub>, <i>y</i><sub class="lower-index">0</sub>, <i>z</i><sub class="lower-index">0</sub>)</span>, and then moves along the polyline at the constant speed <span class="tex-span"><i>v</i><sub class="lower-index"><i>s</i></sub></span>. The twins have not yet found out how the snitch behaves then. Nevertheless, they hope that the retrieved information will help Harry Potter and his team in the upcoming match against Slytherin. Harry Potter learned that at the beginning the game he will be at the point <span class="tex-span">(<i>P</i><sub class="lower-index"><i>x</i></sub>, <i>P</i><sub class="lower-index"><i>y</i></sub>, <i>P</i><sub class="lower-index"><i>z</i></sub>)</span> and his super fast Nimbus 2011 broom allows him to move at the constant speed <span class="tex-span"><i>v</i><sub class="lower-index"><i>p</i></sub></span> in any direction or remain idle. <span class="tex-span"><i>v</i><sub class="lower-index"><i>p</i></sub></span> is not less than the speed of the snitch <span class="tex-span"><i>v</i><sub class="lower-index"><i>s</i></sub></span>. Harry Potter, of course, wants to catch the snitch as soon as possible. Or, if catching the snitch while it is moving along the polyline is impossible, he wants to hurry the Weasley brothers with their experiments. Harry Potter catches the snitch at the time when they are at the same point. Help Harry.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10000</span>). The following <span class="tex-span"><i>n</i> + 1</span> lines contain the coordinates <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>z</i><sub class="lower-index"><i>i</i></sub></span>, separated by single spaces. The coordinates of any two consecutive points do not coincide. The next line contains the velocities <span class="tex-span"><i>v</i><sub class="lower-index"><i>p</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>s</i></sub></span>, the last line contains <span class="tex-span"><i>P</i><sub class="lower-index"><i>x</i></sub></span>, <span class="tex-span"><i>P</i><sub class="lower-index"><i>y</i></sub></span>, <span class="tex-span"><i>P</i><sub class="lower-index"><i>z</i></sub></span>, separated by single spaces. All the numbers in the input are integers, their absolute value does not exceed <span class="tex-span">10<sup class="upper-index">4</sup></span>. The speeds are strictly positive. It is guaranteed that <span class="tex-span"><i>v</i><sub class="lower-index"><i>s</i></sub> ≤ <i>v</i><sub class="lower-index"><i>p</i></sub></span>.</p></div><div class="output-specification"><p>If Harry Potter can catch the snitch while it is moving along the polyline (including the end <span class="tex-span">(<i>x</i><sub class="lower-index"><i>n</i></sub>, <i>y</i><sub class="lower-index"><i>n</i></sub>, <i>z</i><sub class="lower-index"><i>n</i></sub>)</span>), print "YES" in the first line (without the quotes). Print in the second line <span class="tex-span"><i>t</i></span>, which is the earliest moment of time, when Harry will be able to catch the snitch. On the third line print three numbers <span class="tex-span"><i>X</i></span>, <span class="tex-span"><i>Y</i></span>, <span class="tex-span"><i>Z</i></span>, the coordinates of the point at which this happens. The absolute or relative error in the answer should not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. If Harry is not able to catch the snitch during its moving along the described polyline, print "NO".</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10000</span>). The following <span class="tex-span"><i>n</i> + 1</span> lines contain the coordinates <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>z</i><sub class="lower-index"><i>i</i></sub></span>, separated by single spaces. The coordinates of any two consecutive points do not coincide. The next line contains the velocities <span class="tex-span"><i>v</i><sub class="lower-index"><i>p</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>s</i></sub></span>, the last line contains <span class="tex-span"><i>P</i><sub class="lower-index"><i>x</i></sub></span>, <span class="tex-span"><i>P</i><sub class="lower-index"><i>y</i></sub></span>, <span class="tex-span"><i>P</i><sub class="lower-index"><i>z</i></sub></span>, separated by single spaces. All the numbers in the input are integers, their absolute value does not exceed <span class="tex-span">10<sup class="upper-index">4</sup></span>. The speeds are strictly positive. It is guaranteed that <span class="tex-span"><i>v</i><sub class="lower-index"><i>s</i></sub> ≤ <i>v</i><sub class="lower-index"><i>p</i></sub></span>.</p>

## Output

<p>If Harry Potter can catch the snitch while it is moving along the polyline (including the end <span class="tex-span">(<i>x</i><sub class="lower-index"><i>n</i></sub>, <i>y</i><sub class="lower-index"><i>n</i></sub>, <i>z</i><sub class="lower-index"><i>n</i></sub>)</span>), print "YES" in the first line (without the quotes). Print in the second line <span class="tex-span"><i>t</i></span>, which is the earliest moment of time, when Harry will be able to catch the snitch. On the third line print three numbers <span class="tex-span"><i>X</i></span>, <span class="tex-span"><i>Y</i></span>, <span class="tex-span"><i>Z</i></span>, the coordinates of the point at which this happens. The absolute or relative error in the answer should not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. If Harry is not able to catch the snitch during its moving along the described polyline, print "NO".</p>





```input1
4
0 0 0
0 10 0
10 10 0
10 0 0
0 0 0
1 1
5 5 25

```




```input2
4
0 0 0
0 10 0
10 10 0
10 0 0
0 0 0
1 1
5 5 50

```




```input3
1
1 2 3
4 5 6
20 10
1 2 3

```




```output1
YES
25.5000000000
10.0000000000 4.5000000000 0.0000000000

```




```output2
NO

```




```output3
YES
0.0000000000
1.0000000000 2.0000000000 3.0000000000

```


