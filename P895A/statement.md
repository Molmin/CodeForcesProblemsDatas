## Description

<div><p>Students Vasya and Petya are studying at the BSU (Byteland State University). At one of the breaks they decided to order a pizza. In this problem pizza is a circle of some radius. The pizza was delivered already cut into <span class="tex-span"><i>n</i></span> pieces. The <span class="tex-span"><i>i</i></span>-th piece is a sector of angle equal to <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. Vasya and Petya want to divide all pieces of pizza into two <span class="tex-font-style-it">continuous</span> sectors in such way that the difference between angles of these sectors is minimal. Sector angle is sum of angles of all pieces in it. Pay attention, that one of sectors can be empty.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 360</span>) &nbsp;— the number of pieces into which the delivered pizza was cut.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 360</span>) &nbsp;— the angles of the sectors into which the pizza was cut. The sum of all <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is 360.</p></div><div class="output-specification"><p>Print one integer &nbsp;— the minimal difference between angles of sectors that will go to Vasya and Petya.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 360</span>) &nbsp;— the number of pieces into which the delivered pizza was cut.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 360</span>) &nbsp;— the angles of the sectors into which the pizza was cut. The sum of all <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is 360.</p>

## Output

<p>Print one integer &nbsp;— the minimal difference between angles of sectors that will go to Vasya and Petya.</p>





```input1
4
90 90 90 90

```




```input2
3
100 100 160

```




```input3
1
360

```




```input4
4
170 30 150 10

```




```output1
0

```




```output2
40

```




```output3
360

```




```output4
0

```



## Note

<p>In first sample Vasya can take <span class="tex-span">1</span> and <span class="tex-span">2</span> pieces, Petya can take <span class="tex-span">3</span> and <span class="tex-span">4</span> pieces. Then the answer is <span class="tex-span">|(90 + 90) - (90 + 90)| = 0</span>.</p><p>In third sample there is only one piece of pizza that can be taken by only one from Vasya and Petya. So the answer is <span class="tex-span">|360 - 0| = 360</span>.</p><p>In fourth sample Vasya can take <span class="tex-span">1</span> and <span class="tex-span">4</span> pieces, then Petya will take <span class="tex-span">2</span> and <span class="tex-span">3</span> pieces. So the answer is <span class="tex-span">|(170 + 10) - (30 + 150)| = 0</span>.</p><p>Picture explaning fourth sample:</p><p><img class="tex-graphics" src="file://SZ7fNDY5.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Both red and green sectors consist of two adjacent pieces of pizza. So Vasya can take green sector, then Petya will take red sector.</p>
