## Description

<div><p>Petya loves volleyball very much. One day he was running late for a volleyball match. Petya hasn't bought his own car yet, that's why he had to take a taxi. The city has <span class="tex-span"><i>n</i></span> junctions, some of which are connected by two-way roads. The length of each road is defined by some positive integer number of meters; the roads can have different lengths.</p><p>Initially each junction has exactly one taxi standing there. The taxi driver from the <span class="tex-span"><i>i</i></span>-th junction agrees to drive Petya (perhaps through several intermediate junctions) to some other junction if the travel distance is not more than <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> meters. Also, the cost of the ride doesn't depend on the distance and is equal to <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> bourles. Taxis can't stop in the middle of a road. <span class="tex-font-style-bf">Each taxi can be used no more than once. Petya can catch taxi only in the junction, where it stands initially.</span></p><p>At the moment Petya is located on the junction <span class="tex-span"><i>x</i></span> and the volleyball stadium is on the junction <span class="tex-span"><i>y</i></span>. Determine the minimum amount of money Petya will need to drive to the stadium.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000, 0 ≤ <i>m</i> ≤ 1000)</span>. They are the number of junctions and roads in the city correspondingly. The junctions are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, inclusive. The next line contains two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i></span>). They are the numbers of the initial and final junctions correspondingly. Next <span class="tex-span"><i>m</i></span> lines contain the roads' description. Each road is described by a group of three integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — they are the numbers of the junctions connected by the road and the length of the road, correspondingly. The next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>n</i></span> pairs of integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), which describe the taxi driver that waits at the <span class="tex-span"><i>i</i></span>-th junction — the maximum distance he can drive and the drive's cost. The road can't connect the junction with itself, but between a pair of junctions there can be more than one road. All consecutive numbers in each line are separated by exactly one space character.</p></div><div class="output-specification"><p>If taxis can't drive Petya to the destination point, print "-1" (without the quotes). Otherwise, print the drive's minimum cost.</p><p>Please do not use the %lld specificator to read or write 64-bit integers in С++. It is preferred to use cin, cout streams or the %I64d specificator.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000, 0 ≤ <i>m</i> ≤ 1000)</span>. They are the number of junctions and roads in the city correspondingly. The junctions are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, inclusive. The next line contains two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i></span>). They are the numbers of the initial and final junctions correspondingly. Next <span class="tex-span"><i>m</i></span> lines contain the roads' description. Each road is described by a group of three integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — they are the numbers of the junctions connected by the road and the length of the road, correspondingly. The next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>n</i></span> pairs of integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), which describe the taxi driver that waits at the <span class="tex-span"><i>i</i></span>-th junction — the maximum distance he can drive and the drive's cost. The road can't connect the junction with itself, but between a pair of junctions there can be more than one road. All consecutive numbers in each line are separated by exactly one space character.</p>

## Output

<p>If taxis can't drive Petya to the destination point, print "-1" (without the quotes). Otherwise, print the drive's minimum cost.</p><p>Please do not use the %lld specificator to read or write 64-bit integers in С++. It is preferred to use cin, cout streams or the %I64d specificator.</p>





```input1
4 4
1 3
1 2 3
1 4 1
2 4 1
2 3 5
2 7
7 2
1 2
7 7

```




```output1
9

```



## Note

<p>An optimal way — ride from the junction 1 to 2 (via junction 4), then from 2 to 3. It costs 7+2=9 bourles.</p>
