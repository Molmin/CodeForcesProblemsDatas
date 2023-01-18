## Description

<div><p>Leonid wants to become a glass carver (the person who creates beautiful artworks by cutting the glass). He already has a rectangular <span class="tex-span"><i>w</i></span> mm <span class="tex-span"> × </span> <span class="tex-span"><i>h</i></span> mm sheet of glass, a diamond glass cutter and lots of enthusiasm. What he lacks is understanding of what to carve and how.</p><p>In order not to waste time, he decided to practice the technique of carving. To do this, he makes vertical and horizontal cuts through the entire sheet. This process results in making smaller rectangular fragments of glass. Leonid does not move the newly made glass fragments. In particular, a cut divides each fragment of glass that it goes through into smaller fragments.</p><p>After each cut Leonid tries to determine what area the largest of the currently available glass fragments has. Since there appear more and more fragments, this question takes him more and more time and distracts him from the fascinating process.</p><p>Leonid offers to divide the labor — he will cut glass, and you will calculate the area of the maximum fragment after each cut. Do you agree?</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>w</i>, <i>h</i>, <i>n</i></span> (<span class="tex-span">2 ≤ <i>w</i>, <i>h</i> ≤ 200 000</span>, <span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>).</p><p>Next <span class="tex-span"><i>n</i></span> lines contain the descriptions of the cuts. Each description has the form <span class="tex-span"><i>H</i>&nbsp;<i>y</i></span> or <span class="tex-span"><i>V</i>&nbsp;<i>x</i></span>. In the first case Leonid makes the horizontal cut at the distance <span class="tex-span"><i>y</i></span> millimeters (<span class="tex-span">1 ≤ <i>y</i> ≤ <i>h</i> - 1</span>) from the lower edge of the original sheet of glass. In the second case Leonid makes a vertical cut at distance <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>w</i> - 1</span>) millimeters from the left edge of the original sheet of glass. It is guaranteed that Leonid won't make two identical cuts.</p></div><div class="output-specification"><p>After each cut print on a single line the area of the maximum available glass fragment in mm<span class="tex-span"><sup class="upper-index">2</sup></span>.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>w</i>, <i>h</i>, <i>n</i></span> (<span class="tex-span">2 ≤ <i>w</i>, <i>h</i> ≤ 200 000</span>, <span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>).</p><p>Next <span class="tex-span"><i>n</i></span> lines contain the descriptions of the cuts. Each description has the form <span class="tex-span"><i>H</i>&nbsp;<i>y</i></span> or <span class="tex-span"><i>V</i>&nbsp;<i>x</i></span>. In the first case Leonid makes the horizontal cut at the distance <span class="tex-span"><i>y</i></span> millimeters (<span class="tex-span">1 ≤ <i>y</i> ≤ <i>h</i> - 1</span>) from the lower edge of the original sheet of glass. In the second case Leonid makes a vertical cut at distance <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>w</i> - 1</span>) millimeters from the left edge of the original sheet of glass. It is guaranteed that Leonid won't make two identical cuts.</p>

## Output

<p>After each cut print on a single line the area of the maximum available glass fragment in mm<span class="tex-span"><sup class="upper-index">2</sup></span>.</p>





```input1
4 3 4
H 2
V 2
V 3
V 1

```




```input2
7 6 5
H 4
V 3
V 5
H 2
V 1

```




```output1
8
4
4
2

```




```output2
28
16
12
6
4

```



## Note

<p>Picture for the first sample test: </p><center> <img class="tex-graphics" src="file://i1aJXQHu.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> Picture for the second sample test: <center> <img class="tex-graphics" src="file://sDMaWNBM.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
