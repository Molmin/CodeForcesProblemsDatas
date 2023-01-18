## Description

<div><p>Flatland has recently introduced a new type of an eye check for the driver's licence. The check goes like that: there is a plane with mannequins standing on it. You should tell the value of the minimum angle with the vertex at the origin of coordinates and with all mannequins standing inside or on the boarder of this angle. </p><p>As you spend lots of time "glued to the screen", your vision is impaired. So you have to write a program that will pass the check for you.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i> (1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of mannequins.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain two space-separated integers each: <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> (|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 1000)</span> — the coordinates of the <span class="tex-span"><i>i</i></span>-th mannequin. It is guaranteed that the origin of the coordinates has no mannequin. It is guaranteed that no two mannequins are located in the same point on the plane.</p></div><div class="output-specification"><p>Print a single real number — the value of the sought angle in degrees. The answer will be considered valid if the relative or absolute error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i> (1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of mannequins.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain two space-separated integers each: <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> (|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 1000)</span> — the coordinates of the <span class="tex-span"><i>i</i></span>-th mannequin. It is guaranteed that the origin of the coordinates has no mannequin. It is guaranteed that no two mannequins are located in the same point on the plane.</p>

## Output

<p>Print a single real number — the value of the sought angle in degrees. The answer will be considered valid if the relative or absolute error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p>





```input1
2
2 0
0 2

```




```input2
3
2 0
0 2
-2 2

```




```input3
4
2 0
0 2
-2 0
0 -2

```




```input4
2
2 1
1 2

```




```output1
90.0000000000

```




```output2
135.0000000000

```




```output3
270.0000000000

```




```output4
36.8698976458

```



## Note

<p>Solution for the first sample test is shown below: </p><center> <img class="tex-graphics" src="file://8ZYLnHNC.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Solution for the second sample test is shown below: </p><center> <img class="tex-graphics" src="file://IUbmbaQO.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Solution for the third sample test is shown below: </p><center> <img class="tex-graphics" src="file://7TlodgqY.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Solution for the fourth sample test is shown below: </p><center> <img class="tex-graphics" src="file://eEQLNgdo.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
