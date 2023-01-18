## Description

<div><p>One day, as Sherlock Holmes was tracking down one very important criminal, he found a wonderful painting on the wall. This wall could be represented as a plane. The painting had several concentric circles that divided the wall into several parts. Some parts were painted red and all the other were painted blue. Besides, any two neighboring parts were painted different colors, that is, the red and the blue color were alternating, i. e. followed one after the other. The outer area of the wall (the area that lied outside all circles) was painted blue. Help Sherlock Holmes determine the total area of red parts of the wall.</p><p><span class="tex-font-style-underline">Let us remind you that two circles are called concentric if their centers coincide. Several circles are called concentric if any two of them are concentric.</span></p></div><div class="input-specification"><p>The first line contains the single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — the circles' radii. It is guaranteed that all circles are different.</p></div><div class="output-specification"><p>Print the single real number — total area of the part of the wall that is painted red. The answer is accepted if absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p></div>

## Input

<p>The first line contains the single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — the circles' radii. It is guaranteed that all circles are different.</p>

## Output

<p>Print the single real number — total area of the part of the wall that is painted red. The answer is accepted if absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p>





```input1
1
1

```




```input2
3
1 4 2

```




```output1
3.1415926536

```




```output2
40.8407044967

```



## Note

<p>In the first sample the picture is just one circle of radius <span class="tex-span">1</span>. Inner part of the circle is painted red. The area of the red part equals <span class="tex-span">π × 1<sup class="upper-index">2</sup> = π</span>.</p><p>In the second sample there are three circles of radii <span class="tex-span">1</span>, <span class="tex-span">4</span> and <span class="tex-span">2</span>. Outside part of the second circle is painted blue. Part between the second and the third circles is painted red. Part between the first and the third is painted blue. And, finally, the inner part of the first circle is painted red. Overall there are two red parts: the ring between the second and the third circles and the inner part of the first circle. Total area of the red parts is equal <span class="tex-span">(π × 4<sup class="upper-index">2</sup> - π × 2<sup class="upper-index">2</sup>) + π × 1<sup class="upper-index">2</sup> = π × 12 + π = 13π</span></p>
