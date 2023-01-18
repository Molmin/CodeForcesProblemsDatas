## Description

<div><p>You've got an <span class="tex-span"><i>n</i> × <i>m</i></span> pixel picture. Each pixel can be white or black. Your task is to change the colors of as few pixels as possible to obtain a barcode picture.</p><p>A picture is a barcode if the following conditions are fulfilled: </p><ul> <li> All pixels in each column are of the same color. </li><li> The width of each monochrome vertical line is at least <span class="tex-span"><i>x</i></span> and at most <span class="tex-span"><i>y</i></span> pixels. In other words, if we group all neighbouring columns of the pixels with equal color, the size of each group can not be less than <span class="tex-span"><i>x</i></span> or greater than <span class="tex-span"><i>y</i></span>. </li></ul></div><div class="input-specification"><p>The first line contains four space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>x</i>, <i>y</i> ≤ 1000;&nbsp;<i>x</i> ≤ <i>y</i></span>).</p><p>Then follow <span class="tex-span"><i>n</i></span> lines, describing the original image. Each of these lines contains exactly <span class="tex-span"><i>m</i></span> characters. Character "<span class="tex-font-style-tt">.</span>" represents a white pixel and "<span class="tex-font-style-tt">#</span>" represents a black pixel. The picture description doesn't have any other characters besides "<span class="tex-font-style-tt">.</span>" and "<span class="tex-font-style-tt">#</span>".</p></div><div class="output-specification"><p>In the first line print the minimum number of pixels to repaint. It is guaranteed that the answer exists. </p></div>

## Input

<p>The first line contains four space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>x</i>, <i>y</i> ≤ 1000;&nbsp;<i>x</i> ≤ <i>y</i></span>).</p><p>Then follow <span class="tex-span"><i>n</i></span> lines, describing the original image. Each of these lines contains exactly <span class="tex-span"><i>m</i></span> characters. Character "<span class="tex-font-style-tt">.</span>" represents a white pixel and "<span class="tex-font-style-tt">#</span>" represents a black pixel. The picture description doesn't have any other characters besides "<span class="tex-font-style-tt">.</span>" and "<span class="tex-font-style-tt">#</span>".</p>

## Output

<p>In the first line print the minimum number of pixels to repaint. It is guaranteed that the answer exists. </p>





```input1
6 5 1 2
##.#.
.###.
###..
#...#
.##.#
###..

```




```input2
2 5 1 1
#####
.....

```




```output1
11

```




```output2
5

```



## Note

<p>In the first test sample the picture after changing some colors can looks as follows: </p><center> <pre class="verbatim"><br>.##..<br>.##..<br>.##..<br>.##..<br>.##..<br>.##..<br></pre> </center><p>In the second test sample the picture after changing some colors can looks as follows: </p><center> <pre class="verbatim"><br>.#.#.<br>.#.#.<br></pre> </center>
