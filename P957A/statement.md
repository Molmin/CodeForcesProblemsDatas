## Description

<div><p>Overlooking the captivating blend of myriads of vernal hues, Arkady the painter lays out a long, long canvas.</p><p>Arkady has a sufficiently large amount of paint of three colours: cyan, magenta, and yellow. On the one-dimensional canvas split into <span class="tex-span"><i>n</i></span> consecutive segments, each segment needs to be painted in one of the colours.</p><p>Arkady has already painted some (possibly none or all) segments and passes the paintbrush to you. You are to determine whether there are at least two ways of colouring all the unpainted segments so that no two adjacent segments are of the same colour. Two ways are considered different if and only if a segment is painted in different colours in them.</p></div><div class="input-specification"><p>The first line contains a single positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the length of the canvas.</p><p>The second line contains a string <span class="tex-span"><i>s</i></span> of <span class="tex-span"><i>n</i></span> characters, the <span class="tex-span"><i>i</i></span>-th of which is either '<span class="tex-font-style-tt">C</span>' (denoting a segment painted in cyan), '<span class="tex-font-style-tt">M</span>' (denoting one painted in magenta), '<span class="tex-font-style-tt">Y</span>' (one painted in yellow), or '<span class="tex-font-style-tt">?</span>' (an unpainted one).</p></div><div class="output-specification"><p>If there are at least two different ways of painting, output "<span class="tex-font-style-tt">Yes</span>"; otherwise output "<span class="tex-font-style-tt">No</span>" (both without quotes).</p><p>You can print each character in any case (upper or lower).</p></div>

## Input

<p>The first line contains a single positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the length of the canvas.</p><p>The second line contains a string <span class="tex-span"><i>s</i></span> of <span class="tex-span"><i>n</i></span> characters, the <span class="tex-span"><i>i</i></span>-th of which is either '<span class="tex-font-style-tt">C</span>' (denoting a segment painted in cyan), '<span class="tex-font-style-tt">M</span>' (denoting one painted in magenta), '<span class="tex-font-style-tt">Y</span>' (one painted in yellow), or '<span class="tex-font-style-tt">?</span>' (an unpainted one).</p>

## Output

<p>If there are at least two different ways of painting, output "<span class="tex-font-style-tt">Yes</span>"; otherwise output "<span class="tex-font-style-tt">No</span>" (both without quotes).</p><p>You can print each character in any case (upper or lower).</p>





```input1
5
CY??Y

```




```input2
5
C?C?Y

```




```input3
5
?CYC?

```




```input4
5
C??MM

```




```input5
3
MMY

```




```output1
Yes

```




```output2
Yes

```




```output3
Yes

```




```output4
No

```




```output5
No

```



## Note

<p>For the first example, there are exactly two different ways of colouring: <span class="tex-font-style-tt">CYCMY</span> and <span class="tex-font-style-tt">CYMCY</span>.</p><p>For the second example, there are also exactly two different ways of colouring: <span class="tex-font-style-tt">CMCMY</span> and <span class="tex-font-style-tt">CYCMY</span>.</p><p>For the third example, there are four ways of colouring: <span class="tex-font-style-tt">MCYCM</span>, <span class="tex-font-style-tt">MCYCY</span>, <span class="tex-font-style-tt">YCYCM</span>, and <span class="tex-font-style-tt">YCYCY</span>.</p><p>For the fourth example, no matter how the unpainted segments are coloured, the existing magenta segments will prevent the painting from satisfying the requirements. The similar is true for the fifth example.</p>
