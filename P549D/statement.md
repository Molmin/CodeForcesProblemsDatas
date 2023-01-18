## Description

<div><p>The first algorithm for detecting a face on the image working in realtime was developed by Paul Viola and Michael Jones in 2001. A part of the algorithm is a procedure that computes <span class="tex-font-style-it">Haar features</span>. As part of this task, we consider a simplified model of this concept.</p><p>Let's consider a rectangular image that is represented with a table of size <span class="tex-span"><i>n</i> × <i>m</i></span>. The table elements are integers that specify the brightness of each pixel in the image.</p><p>A <span class="tex-font-style-it">feature</span> also is a rectangular table of size <span class="tex-span"><i>n</i> × <i>m</i></span>. Each cell of a <span class="tex-font-style-it">feature</span> is painted black or white.</p><p>To calculate the value of the given feature at the given image, you must perform the following steps. First the table of the feature is put over the table of the image (without rotations or reflections), thus each pixel is entirely covered with either black or white cell. The <span class="tex-font-style-it">value</span> of a feature in the image is the value of <span class="tex-span"><i>W</i> - <i>B</i></span>, where <span class="tex-span"><i>W</i></span> is the total brightness of the pixels in the image, covered with white feature cells, and <span class="tex-span"><i>B</i></span> is the total brightness of the pixels covered with black feature cells.</p><p>Some examples of the most popular Haar features are given below. </p><center> <img class="tex-graphics" src="file://AsNtrgNn.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Your task is to determine the number of operations that are required to calculate the feature by using the so-called <span class="tex-font-style-it">prefix rectangles</span>.</p><p>A <span class="tex-font-style-it">prefix rectangle</span> is any rectangle on the image, the upper left corner of which coincides with the upper left corner of the image.</p><p>You have a variable <span class="tex-span"><i>value</i></span>, whose value is initially zero. In one <span class="tex-font-style-it">operation</span> you can count the sum of pixel values ​​at any prefix rectangle, multiply it by any integer and add to variable <span class="tex-span"><i>value</i></span>.</p><p>You are given a feature. It is necessary to calculate the minimum number of <span class="tex-font-style-it">operations</span> required to calculate the values of this attribute at an arbitrary image. For a better understanding of the statement, read the explanation of the first sample.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>) — the number of rows and columns in the feature.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain the description of the feature. Each line consists of <span class="tex-span"><i>m</i></span> characters, the <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th line equals to "<span class="tex-font-style-tt">W</span>", if this element of the feature is white and "<span class="tex-font-style-tt">B</span>" if it is black.</p></div><div class="output-specification"><p>Print a single number — the minimum number of operations that you need to make to calculate the value of the feature.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>) — the number of rows and columns in the feature.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain the description of the feature. Each line consists of <span class="tex-span"><i>m</i></span> characters, the <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th line equals to "<span class="tex-font-style-tt">W</span>", if this element of the feature is white and "<span class="tex-font-style-tt">B</span>" if it is black.</p>

## Output

<p>Print a single number — the minimum number of operations that you need to make to calculate the value of the feature.</p>





```input1
6 8
BBBBBBBB
BBBBBBBB
BBBBBBBB
WWWWWWWW
WWWWWWWW
WWWWWWWW

```




```input2
3 3
WBW
BWW
WWW

```




```input3
3 6
WWBBWW
WWBBWW
WWBBWW

```




```input4
4 4
BBBB
BBBB
BBBB
BBBW

```




```output1
2

```




```output2
4

```




```output3
3

```




```output4
4

```



## Note

<p>The first sample corresponds to feature <span class="tex-span"><i>B</i></span>, the one shown in the picture. The value of this feature in an image of size <span class="tex-span">6 × 8</span> equals to the difference of the total brightness of the pixels in the lower and upper half of the image. To calculate its value, perform the following two <span class="tex-font-style-it">operations</span>:</p><ol> <li> add the sum of pixels in the prefix rectangle with the lower right corner in the <span class="tex-span">6</span>-th row and <span class="tex-span">8</span>-th column with coefficient <span class="tex-span">1</span> to the variable <span class="tex-span"><i>value</i></span> (the rectangle is indicated by a red frame); <img class="tex-graphics" src="file://sVwU7Kkn.png" style="max-width: 100.0%;max-height: 100.0%;"></li><li> add the number of pixels in the prefix rectangle with the lower right corner in the <span class="tex-span">3</span>-rd row and <span class="tex-span">8</span>-th column with coefficient <span class="tex-span"> - 2</span> and variable <span class="tex-span"><i>value</i></span>. <img class="tex-graphics" src="file://T4KUxdv6.png" style="max-width: 100.0%;max-height: 100.0%;"> </li></ol><p>Thus, all the pixels in the lower three rows of the image will be included with factor <span class="tex-span">1</span>, and all pixels in the upper three rows of the image will be included with factor <span class="tex-span">1 - 2 =  - 1</span>, as required.</p>
