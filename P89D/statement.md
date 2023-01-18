## Description

<div><p>Once upon a time in the galaxy of far, far away...</p><p>Darth Wader found out the location of a rebels' base. Now he is going to destroy the base (and the whole planet that the base is located at), using the Death Star.</p><p>When the rebels learnt that the Death Star was coming, they decided to use their new secret weapon — space mines. Let's describe a space mine's build.</p><p>Each space mine is shaped like a ball (we'll call it the mine body) of a certain radius <span class="tex-span"><i>r</i></span> with the center in the point <span class="tex-span"><i>O</i></span>. Several spikes protrude from the center. Each spike can be represented as a segment, connecting the center of the mine with some point <span class="tex-span"><i>P</i></span>, such that <img align="middle" class="tex-formula" src="file://hA6rhKl1.png" style="max-width: 100.0%;max-height: 100.0%;"> (transporting long-spiked mines is problematic), where <span class="tex-span">|<i>OP</i>|</span> is the length of the segment connecting <span class="tex-span"><i>O</i></span> and <span class="tex-span"><i>P</i></span>. It is convenient to describe the point <span class="tex-span"><i>P</i></span> by a vector <span class="tex-span"><i>p</i></span> such that <span class="tex-span"><i>P</i> = <i>O</i> + <i>p</i></span>.</p><p>The Death Star is shaped like a ball with the radius of <span class="tex-span"><i>R</i></span> (<span class="tex-span"><i>R</i></span> exceeds any mine's radius). It moves at a constant speed along the <span class="tex-span"><i>v</i></span> vector at the speed equal to <span class="tex-span">|<i>v</i>|</span>. At the moment the rebels noticed the Star of Death, it was located in the point <span class="tex-span"><i>A</i></span>.</p><p>The rebels located <span class="tex-span"><i>n</i></span> space mines along the Death Star's way. You may regard the mines as being idle. The Death Star does not know about the mines' existence and cannot notice them, which is why it doesn't change the direction of its movement. As soon as the Star of Death touched the mine (its body or one of the spikes), the mine bursts and destroys the Star of Death. A touching is the situation when there is a point in space which belongs both to the mine and to the Death Star. It is considered that Death Star will not be destroyed if it can move infinitely long time without touching the mines.</p><p>Help the rebels determine whether they will succeed in destroying the Death Star using space mines or not. If they will succeed, determine the moment of time when it will happen (starting from the moment the Death Star was noticed).</p></div><div class="input-specification"><p>The first input data line contains <span class="tex-span">7</span> integers <span class="tex-span"><i>A</i><sub class="lower-index"><i>x</i></sub>, <i>A</i><sub class="lower-index"><i>y</i></sub>, <i>A</i><sub class="lower-index"><i>z</i></sub>, <i>v</i><sub class="lower-index"><i>x</i></sub>, <i>v</i><sub class="lower-index"><i>y</i></sub>, <i>v</i><sub class="lower-index"><i>z</i></sub>, <i>R</i></span>. They are the Death Star's initial position, the direction of its movement, and its radius (<span class="tex-span"> - 10 ≤ <i>v</i><sub class="lower-index"><i>x</i></sub>, <i>v</i><sub class="lower-index"><i>y</i></sub>, <i>v</i><sub class="lower-index"><i>z</i></sub> ≤ 10</span>, <span class="tex-span">|<i>v</i>| &gt; 0</span>, <span class="tex-span">0 &lt; <i>R</i> ≤ 100</span>).</p><p>The second line contains an integer <span class="tex-span"><i>n</i></span>, which is the number of mines (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). Then follow <span class="tex-span"><i>n</i></span> data blocks, the <span class="tex-span"><i>i</i></span>-th of them describes the <span class="tex-span"><i>i</i></span>-th mine.</p><p>The first line of each block contains <span class="tex-span">5</span> integers <span class="tex-span"><i>O</i><sub class="lower-index"><i>ix</i></sub>, <i>O</i><sub class="lower-index"><i>iy</i></sub>, <i>O</i><sub class="lower-index"><i>iz</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>m</i><sub class="lower-index"><i>i</i></sub></span>, which are the coordinates of the mine centre, the radius of its body and the number of spikes (<span class="tex-span">0 &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> &lt; 100, 0 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ 10</span>). Then follow <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> lines, describing the spikes of the <span class="tex-span"><i>i</i></span>-th mine, where the <span class="tex-span"><i>j</i></span>-th of them describes the <span class="tex-span"><i>i</i></span>-th spike and contains <span class="tex-span">3</span> integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>ijx</i></sub>, <i>p</i><sub class="lower-index"><i>ijy</i></sub>, <i>p</i><sub class="lower-index"><i>ijz</i></sub></span> — the coordinates of the vector where the given spike is directed (<img align="middle" class="tex-formula" src="file://VBwBdFws.png" style="max-width: 100.0%;max-height: 100.0%;">).</p><p>The coordinates of the mines' centers and the center of the Death Star are integers, their absolute value does not exceed <span class="tex-span">10000</span>. It is guaranteed that <span class="tex-span"><i>R</i> &gt; <i>r</i><sub class="lower-index"><i>i</i></sub></span> for any <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>. For any mines <span class="tex-span"><i>i</i> ≠ <i>j</i></span> the following inequality if fulfilled: <img align="middle" class="tex-formula" src="file://A8kGUkoo.png" style="max-width: 100.0%;max-height: 100.0%;">. Initially the Death Star and the mines do not have common points.</p></div><div class="output-specification"><p>If the rebels will succeed in stopping the Death Star using space mines, print the time from the moment the Death Star was noticed to the blast.</p><p>If the Death Star will not touch a mine, print "-1" (without quotes).</p><p>For the answer the absolute or relative error of <span class="tex-span">10<sup class="upper-index"> - 6</sup></span> is acceptable.</p></div>

## Input

<p>The first input data line contains <span class="tex-span">7</span> integers <span class="tex-span"><i>A</i><sub class="lower-index"><i>x</i></sub>, <i>A</i><sub class="lower-index"><i>y</i></sub>, <i>A</i><sub class="lower-index"><i>z</i></sub>, <i>v</i><sub class="lower-index"><i>x</i></sub>, <i>v</i><sub class="lower-index"><i>y</i></sub>, <i>v</i><sub class="lower-index"><i>z</i></sub>, <i>R</i></span>. They are the Death Star's initial position, the direction of its movement, and its radius (<span class="tex-span"> - 10 ≤ <i>v</i><sub class="lower-index"><i>x</i></sub>, <i>v</i><sub class="lower-index"><i>y</i></sub>, <i>v</i><sub class="lower-index"><i>z</i></sub> ≤ 10</span>, <span class="tex-span">|<i>v</i>| &gt; 0</span>, <span class="tex-span">0 &lt; <i>R</i> ≤ 100</span>).</p><p>The second line contains an integer <span class="tex-span"><i>n</i></span>, which is the number of mines (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). Then follow <span class="tex-span"><i>n</i></span> data blocks, the <span class="tex-span"><i>i</i></span>-th of them describes the <span class="tex-span"><i>i</i></span>-th mine.</p><p>The first line of each block contains <span class="tex-span">5</span> integers <span class="tex-span"><i>O</i><sub class="lower-index"><i>ix</i></sub>, <i>O</i><sub class="lower-index"><i>iy</i></sub>, <i>O</i><sub class="lower-index"><i>iz</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>m</i><sub class="lower-index"><i>i</i></sub></span>, which are the coordinates of the mine centre, the radius of its body and the number of spikes (<span class="tex-span">0 &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> &lt; 100, 0 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ 10</span>). Then follow <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> lines, describing the spikes of the <span class="tex-span"><i>i</i></span>-th mine, where the <span class="tex-span"><i>j</i></span>-th of them describes the <span class="tex-span"><i>i</i></span>-th spike and contains <span class="tex-span">3</span> integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>ijx</i></sub>, <i>p</i><sub class="lower-index"><i>ijy</i></sub>, <i>p</i><sub class="lower-index"><i>ijz</i></sub></span> — the coordinates of the vector where the given spike is directed (<img align="middle" class="tex-formula" src="file://VBwBdFws.png" style="max-width: 100.0%;max-height: 100.0%;">).</p><p>The coordinates of the mines' centers and the center of the Death Star are integers, their absolute value does not exceed <span class="tex-span">10000</span>. It is guaranteed that <span class="tex-span"><i>R</i> &gt; <i>r</i><sub class="lower-index"><i>i</i></sub></span> for any <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>. For any mines <span class="tex-span"><i>i</i> ≠ <i>j</i></span> the following inequality if fulfilled: <img align="middle" class="tex-formula" src="file://A8kGUkoo.png" style="max-width: 100.0%;max-height: 100.0%;">. Initially the Death Star and the mines do not have common points.</p>

## Output

<p>If the rebels will succeed in stopping the Death Star using space mines, print the time from the moment the Death Star was noticed to the blast.</p><p>If the Death Star will not touch a mine, print "-1" (without quotes).</p><p>For the answer the absolute or relative error of <span class="tex-span">10<sup class="upper-index"> - 6</sup></span> is acceptable.</p>





```input1
0 0 0 1 0 0 5
2
10 8 0 2 2
0 -3 0
2 2 0
20 0 0 4 3
2 4 0
-4 3 0
1 -5 0

```




```input2
8 8 4 4 4 2 6
1
-2 -2 -1 3 0

```




```input3
30 30 2 1 2 1 20
3
0 0 40 5 1
1 4 4
-10 -40 -5 7 0
100 200 95 8 1
-10 0 0

```




```output1
10.0000000000
```




```output2
-1
```




```output3
74.6757620881
```


