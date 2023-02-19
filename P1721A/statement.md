## Description

<div><p>You have an image file of size $2 \times 2$, consisting of $4$ pixels. Each pixel can have one of $26$ different colors, denoted by lowercase Latin letters.</p><p>You want to recolor some of the pixels of the image <span class="tex-font-style-bf">so that all $4$ pixels have the same color</span>. In one move, you can choose <span class="tex-font-style-bf">no more than two</span> pixels <span class="tex-font-style-bf">of the same color</span> and paint them into some other color <span class="tex-font-style-bf">(if you choose two pixels, both should be painted into the same color)</span>.</p><p>What is the minimum number of moves you have to make in order to fulfill your goal?</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 1000$) — the number of test cases.</p><p>Each test case consists of two lines. Each of these lines contains two lowercase letters of Latin alphabet <span class="tex-font-style-bf">without any separators</span>, denoting a row of pixels in the image.</p></div><div class="output-specification"><p>For each test case, print one integer — the minimum number of moves you have to make so that all $4$ pixels of the image have the same color.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 1000$) — the number of test cases.</p><p>Each test case consists of two lines. Each of these lines contains two lowercase letters of Latin alphabet <span class="tex-font-style-bf">without any separators</span>, denoting a row of pixels in the image.</p>

## Output

<p>For each test case, print one integer — the minimum number of moves you have to make so that all $4$ pixels of the image have the same color.</p>





```input1|2,3,6,7,10,11
5
rb
br
cc
wb
aa
aa
ab
cd
yy
xx
```




```output1
1
2
0
3
1
```



## Note

<p>Let's analyze the test cases of the example.</p><p>In the first test case, you can paint the bottom left pixel and the top right pixel (which share the same color) into the color <span class="tex-font-style-tt">r</span>, so all pixels have this color.</p><p>In the second test case, two moves are enough:</p><ul> <li> paint both top pixels, which have the same color <span class="tex-font-style-tt">c</span>, into the color <span class="tex-font-style-tt">b</span>; </li><li> paint the bottom left pixel into the color <span class="tex-font-style-tt">b</span>. </li></ul><p>In the third test case, all pixels already have the same color.</p><p>In the fourth test case, you may leave any of the pixels unchanged, and paint all three other pixels into the color of that pixel in three moves.</p><p>In the fifth test case, you can paint both top pixels into the color <span class="tex-font-style-tt">x</span>.</p>
