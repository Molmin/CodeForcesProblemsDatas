## Description

<div><p>A country called Flatland is an infinite two-dimensional plane. Flatland has <span class="tex-span"><i>n</i></span> cities, each of them is a point on the plane.</p><p>Flatland is ruled by king Circle IV. Circle IV has 9 sons. He wants to give each of his sons part of Flatland to rule. For that, he wants to draw four <span class="tex-font-style-bf">distinct</span> straight lines, such that two of them are parallel to the <span class="tex-span"><i>Ox</i></span> axis, and two others are parallel to the <span class="tex-span"><i>Oy</i></span> axis. At that, no straight line can go through any city. Thus, Flatland will be divided into 9 parts, and each son will be given exactly one of these parts. Circle IV thought a little, evaluated his sons' obedience and decided that the <span class="tex-span"><i>i</i></span>-th son should get the part of Flatland that has exactly <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> cities.</p><p>Help Circle find such four straight lines that if we divide Flatland into 9 parts by these lines, the resulting parts can be given to the sons so that son number <span class="tex-span"><i>i</i></span> got the part of Flatland which contains <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> cities.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i> (9 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of cities in Flatland. Next <span class="tex-span"><i>n</i></span> lines each contain two space-separated integers: <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ( - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — the coordinates of the <span class="tex-span"><i>i</i></span>-th city. No two cities are located at the same point. The last line contains nine space-separated integers: <img align="middle" class="tex-formula" src="file://fhBArMbv.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div><div class="output-specification"><p>If there is no solution, print a single integer -1.</p><p>Otherwise, print in the first line two distinct real space-separated numbers: <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub></span> — the abscissas of the straight lines that are parallel to the <span class="tex-span"><i>Oy</i></span> axis. And in the second line print two distinct real space-separated numbers: <span class="tex-span"><i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub></span> — the ordinates of the straight lines, parallel to the <span class="tex-span"><i>Ox</i></span>. If there are multiple solutions, print any of them. </p><p>When the answer is being checked, a city is considered to lie on a straight line, if the distance between the city and the line doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. Two straight lines are considered the same if the distance between them doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i> (9 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of cities in Flatland. Next <span class="tex-span"><i>n</i></span> lines each contain two space-separated integers: <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ( - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — the coordinates of the <span class="tex-span"><i>i</i></span>-th city. No two cities are located at the same point. The last line contains nine space-separated integers: <img align="middle" class="tex-formula" src="file://fhBArMbv.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>

## Output

<p>If there is no solution, print a single integer -1.</p><p>Otherwise, print in the first line two distinct real space-separated numbers: <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub></span> — the abscissas of the straight lines that are parallel to the <span class="tex-span"><i>Oy</i></span> axis. And in the second line print two distinct real space-separated numbers: <span class="tex-span"><i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub></span> — the ordinates of the straight lines, parallel to the <span class="tex-span"><i>Ox</i></span>. If there are multiple solutions, print any of them. </p><p>When the answer is being checked, a city is considered to lie on a straight line, if the distance between the city and the line doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. Two straight lines are considered the same if the distance between them doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
9
1 1
1 2
1 3
2 1
2 2
2 3
3 1
3 2
3 3
1 1 1 1 1 1 1 1 1

```




```input2
15
4 4
-1 -3
1 5
3 -4
-4 4
-1 1
3 -3
-4 -5
-3 3
3 2
4 1
-4 2
-2 -5
-3 4
-1 4
2 1 2 1 2 1 3 2 1

```




```input3
10
-2 10
6 0
-16 -6
-4 13
-4 -2
-17 -10
9 15
18 16
-5 2
10 -5
2 1 1 1 1 1 1 1 1

```




```output1
1.5000000000 2.5000000000
1.5000000000 2.5000000000

```




```output2
-3.5000000000 2.0000000000
3.5000000000 -1.0000000000

```




```output3
-1

```



## Note

<p>The solution for the first sample test is shown below:</p><center> <img class="tex-graphics" src="file://ZA8iCqik.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The solution for the second sample test is shown below:</p><center> <img class="tex-graphics" src="file://M1ryXugs.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>There is no solution for the third sample test.</p>
