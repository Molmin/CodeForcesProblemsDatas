## Description

<div><p>Edo has got a collection of <span class="tex-span"><i>n</i></span> refrigerator magnets!</p><p>He decided to buy a refrigerator and hang the magnets on the door. The shop can make the refrigerator with any size of the door that meets the following restrictions: the refrigerator door must be rectangle, and both the length and the width of the door must be <span class="tex-font-style-bf">positive integers</span>.</p><p>Edo figured out how he wants to place the magnets on the refrigerator. He introduced a system of coordinates on the plane, where each magnet is represented as a rectangle with sides parallel to the coordinate axes.</p><p>Now he wants to remove no more than <span class="tex-span"><i>k</i></span> magnets (he may choose to keep all of them) and attach all remaining magnets to the refrigerator door, and the area of ​​the door should be as small as possible. A magnet is considered to be attached to the refrigerator door if <span class="tex-font-style-bf">its center</span> lies on the door or on its boundary. The relative positions of all the remaining magnets must correspond to the plan.</p><p>Let us explain the last two sentences. Let's suppose we want to hang two magnets on the refrigerator. If the magnet in the plan has coordinates of the lower left corner (<span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>) and the upper right corner (<span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span>), then its center is located at (<img align="middle" class="tex-formula" src="file://0sCM7dyT.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://gKFk6pJe.png" style="max-width: 100.0%;max-height: 100.0%;">) (may not be integers). By saying the relative position should correspond to the plan we mean that the only available operation is translation, i.e. the vector connecting the centers of two magnets in the original plan, must be equal to the vector connecting the centers of these two magnets on the refrigerator.</p><p><span class="tex-font-style-bf">The sides of the refrigerator door must also be parallel to coordinate axes.</span></p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ <i>min</i>(10, <i>n</i> - 1)</span>)&nbsp;— the number of magnets that Edo has and the maximum number of magnets Edo may not place on the refrigerator.</p><p>Next <span class="tex-span"><i>n</i></span> lines describe the initial plan of placing magnets. Each line contains four integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1</sub> &lt; <i>x</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index">1</sub> &lt; <i>y</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the coordinates of the lower left and upper right corners of the current magnet. The magnets can partially overlap or even fully coincide.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the minimum area of the door of refrigerator, which can be used to place at least <span class="tex-span"><i>n</i> - <i>k</i></span> magnets, preserving the relative positions. </p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ <i>min</i>(10, <i>n</i> - 1)</span>)&nbsp;— the number of magnets that Edo has and the maximum number of magnets Edo may not place on the refrigerator.</p><p>Next <span class="tex-span"><i>n</i></span> lines describe the initial plan of placing magnets. Each line contains four integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1</sub> &lt; <i>x</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index">1</sub> &lt; <i>y</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the coordinates of the lower left and upper right corners of the current magnet. The magnets can partially overlap or even fully coincide.</p>

## Output

<p>Print a single integer&nbsp;— the minimum area of the door of refrigerator, which can be used to place at least <span class="tex-span"><i>n</i> - <i>k</i></span> magnets, preserving the relative positions. </p>





```input1
3 1
1 1 2 2
2 2 3 3
3 3 4 4

```




```input2
4 1
1 1 2 2
1 9 2 10
9 9 10 10
9 1 10 2

```




```input3
3 0
1 1 2 2
1 1 1000000000 1000000000
1 3 8 12

```




```output1
1

```




```output2
64

```




```output3
249999999000000001

```



## Note

<p>In the first test sample it is optimal to remove either the first or the third magnet. If we remove the first magnet, the centers of two others will lie at points (2.5, 2.5) and (3.5, 3.5). Thus, it is enough to buy a fridge with door width 1 and door height 1, the area of the door also equals one, correspondingly.</p><p>In the second test sample it doesn't matter which magnet to remove, the answer will not change — we need a fridge with door width 8 and door height 8.</p><p>In the third sample you cannot remove anything as <span class="tex-span"><i>k</i> = 0</span>.</p>
