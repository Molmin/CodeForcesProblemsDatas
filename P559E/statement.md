## Description

<div><p>The main walking trail in Geraldion is absolutely straight, and it passes strictly from the north to the south, it is so long that no one has ever reached its ends in either of the two directions. The Geraldionians love to walk on this path at any time, so the mayor of the city asked the Herald to illuminate this path with a few spotlights. The spotlights have already been delivered to certain places and Gerald will not be able to move them. Each spotlight illuminates a specific segment of the path of the given length, one end of the segment is the location of the spotlight, and it can be directed so that it covers the segment to the south or to the north of spotlight.</p><p>The trail contains a monument to the mayor of the island, and although you can walk in either directions from the monument, no spotlight is south of the monument.</p><p>You are given the positions of the spotlights and their power. Help Gerald direct all the spotlights so that the total length of the illuminated part of the path is as much as possible.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of spotlights. Each of the <span class="tex-span"><i>n</i></span> lines contains two space-separated integers, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>, <span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>). Number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> shows how much further the <span class="tex-span"><i>i</i></span>-th spotlight to the north, and number <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> shows the length of the segment it illuminates.</p><p>It is guaranteed that all the <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>'s are distinct.</p></div><div class="output-specification"><p>Print a single integer — the maximum total length of the illuminated part of the path.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of spotlights. Each of the <span class="tex-span"><i>n</i></span> lines contains two space-separated integers, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>, <span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>). Number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> shows how much further the <span class="tex-span"><i>i</i></span>-th spotlight to the north, and number <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> shows the length of the segment it illuminates.</p><p>It is guaranteed that all the <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>'s are distinct.</p>

## Output

<p>Print a single integer — the maximum total length of the illuminated part of the path.</p>





```input1
3
1 1
2 2
3 3

```




```input2
4
1 2
3 3
4 3
6 2

```




```output1
5

```




```output2
9

```


