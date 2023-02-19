## Description

<div><p>Arkadiy has lots square photos with size <span class="tex-span"><i>a</i> × <i>a</i></span>. He wants to put some of them on a rectangular wall with size <span class="tex-span"><i>h</i> × <i>w</i></span>. </p><p>The photos which Arkadiy will put on the wall must form a rectangular grid and the distances between neighboring vertically and horizontally photos and also the distances between outside rows and columns of photos to the nearest bound of the wall must be equal to <span class="tex-span"><i>x</i></span>, where <span class="tex-span"><i>x</i></span> is some non-negative <span class="tex-font-style-bf">real</span> number. Look on the picture below for better understanding of the statement.</p><center> <img class="tex-graphics" src="file://g5rbhzqf.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Arkadiy haven't chosen yet how many photos he would put on the wall, however, he want to put at least one photo. Your task is to determine the <span class="tex-font-style-bf">minimum</span> value of <span class="tex-span"><i>x</i></span> which can be obtained after putting photos, or report that there is no way to put positive number of photos and satisfy all the constraints. Suppose that Arkadiy has enough photos to make any valid arrangement according to the constraints.</p><p>Note that Arkadiy wants to put at least one photo on the wall. The photos should not overlap, should completely lie inside the wall bounds and should have sides parallel to the wall sides.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>h</i></span> and <span class="tex-span"><i>w</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>h</i>, <i>w</i> ≤ 10<sup class="upper-index">9</sup></span>) — the size of photos and the height and the width of the wall.</p></div><div class="output-specification"><p>Print one non-negative real number — the minimum value of <span class="tex-span"><i>x</i></span> which can be obtained after putting the photos on the wall. The absolute or the relative error of the answer must not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p><p>Print <span class="tex-font-style-tt">-1</span> if there is no way to put positive number of photos and satisfy the constraints.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>h</i></span> and <span class="tex-span"><i>w</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>h</i>, <i>w</i> ≤ 10<sup class="upper-index">9</sup></span>) — the size of photos and the height and the width of the wall.</p>

## Output

<p>Print one non-negative real number — the minimum value of <span class="tex-span"><i>x</i></span> which can be obtained after putting the photos on the wall. The absolute or the relative error of the answer must not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p><p>Print <span class="tex-font-style-tt">-1</span> if there is no way to put positive number of photos and satisfy the constraints.</p>





```input1
2 18 13

```




```input2
4 4 4

```




```input3
3 4 3

```




```output1
0.5

```




```output2
0

```




```output3
-1

```



## Note

<p>In the first example Arkadiy can put <span class="tex-span">7</span> rows of photos with <span class="tex-span">5</span> photos in each row, so the minimum value of <span class="tex-span"><i>x</i></span> equals to <span class="tex-span">0.5</span>.</p><p>In the second example Arkadiy can put only <span class="tex-span">1</span> photo which will take the whole wall, so the minimum value of <span class="tex-span"><i>x</i></span> equals to <span class="tex-span">0</span>.</p><p>In the third example there is no way to put positive number of photos and satisfy the constraints described in the statement, so the answer is <span class="tex-font-style-tt">-1</span>.</p>
