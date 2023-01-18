## Description

<div><p>The developers of Looksery have to write an efficient algorithm that detects faces on a picture. Unfortunately, they are currently busy preparing a contest for you, so you will have to do it for them. </p><p>In this problem an image is a rectangular table that consists of lowercase Latin letters. A face on the image is a <span class="tex-span">2 × 2</span> square, such that from the four letters of this square you can make word "<span class="tex-font-style-tt">face</span>". </p><p>You need to write a program that determines the number of faces on the image. The squares that correspond to the faces can overlap.</p></div><div class="input-specification"><p>The first line contains two space-separated integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 50</span>) — the height and the width of the image, respectively.</p><p>Next <span class="tex-span"><i>n</i></span> lines define the image. Each line contains <span class="tex-span"><i>m</i></span> lowercase Latin letters.</p></div><div class="output-specification"><p>In the single line print the number of faces on the image.</p></div>

## Input

<p>The first line contains two space-separated integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 50</span>) — the height and the width of the image, respectively.</p><p>Next <span class="tex-span"><i>n</i></span> lines define the image. Each line contains <span class="tex-span"><i>m</i></span> lowercase Latin letters.</p>

## Output

<p>In the single line print the number of faces on the image.</p>





```input1
4 4
xxxx
xfax
xcex
xxxx

```




```input2
4 2
xx
cf
ae
xx

```




```input3
2 3
fac
cef

```




```input4
1 4
face

```




```output1
1

```




```output2
1

```




```output3
2

```




```output4
0

```



## Note

<p>In the first sample the image contains a single face, located in a square with the upper left corner at the second line and the second column: </p><center> <img class="tex-graphics" src="file://8YEjjvlD.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second sample the image also contains exactly one face, its upper left corner is at the second row and the first column.</p><p>In the third sample two faces are shown: </p><center> <img class="tex-graphics" src="file://LRBIafVe.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the fourth sample the image has no faces on it.</p>
