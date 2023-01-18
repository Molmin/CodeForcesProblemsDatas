## Description

<div><p>Innokenty works at a flea market and sells some <span class="tex-font-style-striked">random stuff</span> rare items. Recently he found an old rectangular blanket. It turned out that the blanket is split in $n \cdot m$ colored pieces that form a rectangle with $n$ rows and $m$ columns. </p><p>The colored pieces attracted Innokenty's attention so he immediately came up with the following business plan. If he cuts out a subrectangle consisting of three colored stripes, he can sell it as a flag of some country. Innokenty decided that a subrectangle is similar enough to a flag of some country if it consists of three stripes of <span class="tex-font-style-bf">equal</span> heights placed one above another, where each stripe consists of cells of equal color. Of course, the color of the top stripe must be different from the color of the middle stripe; and the color of the middle stripe must be different from the color of the bottom stripe.</p><p>Innokenty has not yet decided what part he will cut out, but he is sure that the flag's boundaries should go along grid lines. Also, Innokenty won't rotate the blanket. Please help Innokenty and count the number of different subrectangles Innokenty can cut out and sell as a flag. Two subrectangles located in different places but forming the same flag are still considered different.</p><center> <img class="tex-graphics" src="file://Uo4irQHt.png" style="max-width: 100.0%;max-height: 100.0%;">&nbsp;<img class="tex-graphics" src="file://95COhp1z.png" style="max-width: 100.0%;max-height: 100.0%;">&nbsp;<img class="tex-graphics" src="file://5iynOWMN.png" style="max-width: 100.0%;max-height: 100.0%;"><p><span class="tex-font-size-small">These subrectangles are flags.</span> </p></center><center> <img class="tex-graphics" src="file://F5mvrU37.png" style="max-width: 100.0%;max-height: 100.0%;">&nbsp;<img class="tex-graphics" src="file://Cy3twXDk.png" style="max-width: 100.0%;max-height: 100.0%;">&nbsp;<img class="tex-graphics" src="file://mTzefa9e.png" style="max-width: 100.0%;max-height: 100.0%;">&nbsp;<img class="tex-graphics" src="file://TBCs0VfS.png" style="max-width: 100.0%;max-height: 100.0%;">&nbsp;<img class="tex-graphics" src="file://z3v1ccmV.png" style="max-width: 100.0%;max-height: 100.0%;">&nbsp;<img class="tex-graphics" src="file://1xmCX7wl.png" style="max-width: 100.0%;max-height: 100.0%;"><p><span class="tex-font-size-small">These subrectangles are not flags.</span> </p></center></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 1\,000$)&nbsp;— the number of rows and the number of columns on the blanket.</p><p>Each of the next $n$ lines contains $m$ lowercase English letters from '<span class="tex-font-style-tt">a</span>' to '<span class="tex-font-style-tt">z</span>' and describes a row of the blanket. Equal letters correspond to equal colors, different letters correspond to different colors.</p></div><div class="output-specification"><p>In the only line print the number of subrectangles which form valid flags.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 1\,000$)&nbsp;— the number of rows and the number of columns on the blanket.</p><p>Each of the next $n$ lines contains $m$ lowercase English letters from '<span class="tex-font-style-tt">a</span>' to '<span class="tex-font-style-tt">z</span>' and describes a row of the blanket. Equal letters correspond to equal colors, different letters correspond to different colors.</p>

## Output

<p>In the only line print the number of subrectangles which form valid flags.</p>





```input1
4 3
aaa
bbb
ccb
ddd
```




```input2
6 1
a
a
b
b
c
c
```




```output1
6
```




```output2
1
```



## Note

<center> <img class="tex-graphics" src="file://V3FMbFef.png" style="max-width: 100.0%;max-height: 100.0%;">&nbsp;<img class="tex-graphics" src="file://P6e1Xc8v.png" style="max-width: 100.0%;max-height: 100.0%;"><p><span class="tex-font-size-small">The selected subrectangles are flags in the first example.</span> </p></center>
