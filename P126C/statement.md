## Description

<div><p>After years of hard work scientists invented an absolutely new e-reader display. The new display has a larger resolution, consumes less energy and its production is cheaper. And besides, one can bend it. The only inconvenience is highly unusual management. For that very reason the developers decided to leave the e-readers' software to programmers.</p><p>The display is represented by <span class="tex-span"><i>n</i> × <i>n</i></span> square of pixels, each of which can be either black or white. The display rows are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> upside down, the columns are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from the left to the right. The display can perform commands like "<span class="tex-span"><i>x</i>, <i>y</i></span>". When a traditional display fulfills such command, it simply inverts a color of <span class="tex-span">(<i>x</i>, <i>y</i>)</span>, where <span class="tex-span"><i>x</i></span> is the row number and <span class="tex-span"><i>y</i></span> is the column number. But in our new display every pixel that belongs to at least one of the segments <span class="tex-span">(<i>x</i>, <i>x</i>) - (<i>x</i>, <i>y</i>)</span> and <span class="tex-span">(<i>y</i>, <i>y</i>) - (<i>x</i>, <i>y</i>)</span> (both ends of both segments are included) inverts a color.</p><p>For example, if initially a display <span class="tex-span">5 × 5</span> in size is absolutely white, then the sequence of commands <span class="tex-span">(1, 4)</span>, <span class="tex-span">(3, 5)</span>, <span class="tex-span">(5, 1)</span>, <span class="tex-span">(3, 3)</span> leads to the following changes:</p><center> <img class="tex-graphics" src="file://msWGX52K.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>You are an e-reader software programmer and you should calculate minimal number of commands needed to display the picture. You can regard all display pixels as initially white.</p></div><div class="input-specification"><p>The first line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>).</p><p>Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>n</i></span> characters each: the description of the picture that needs to be shown. "<span class="tex-font-style-tt">0</span>" represents the white color and "<span class="tex-font-style-tt">1</span>" represents the black color. </p></div><div class="output-specification"><p>Print one integer <span class="tex-span"><i>z</i></span> — the least number of commands needed to display the picture.</p></div>

## Input

<p>The first line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>).</p><p>Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>n</i></span> characters each: the description of the picture that needs to be shown. "<span class="tex-font-style-tt">0</span>" represents the white color and "<span class="tex-font-style-tt">1</span>" represents the black color. </p>

## Output

<p>Print one integer <span class="tex-span"><i>z</i></span> — the least number of commands needed to display the picture.</p>





```input1
5
01110
10010
10001
10011
11110

```




```output1
4

```


