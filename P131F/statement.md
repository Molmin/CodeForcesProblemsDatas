## Description

<div><p>How many stars are there in the sky? A young programmer Polycarpus can't get this question out of his head! He took a photo of the starry sky using his digital camera and now he analyzes the resulting monochrome digital picture. The picture is represented by a rectangular matrix consisting of <span class="tex-span"><i>n</i></span> lines each containing <span class="tex-span"><i>m</i></span> characters. A character equals '<span class="tex-font-style-tt">1</span>', if the corresponding photo pixel is white and '<span class="tex-font-style-tt">0</span>', if it is black.</p><p>Polycarpus thinks that he has found a star on the photo if he finds a white pixel surrounded by four side-neighboring pixels that are also white: </p><center> <pre class="verbatim"><br> 1 <br>111<br> 1 <br></pre> <span class="tex-font-size-small">a star on the photo</span> </center><p>Polycarpus whats to cut out a rectangular area from the photo and give his mom as a present. This area should contain no less than <span class="tex-span"><i>k</i></span> stars. The stars can intersect, have shared white pixels on the photo. The boy will cut out the rectangular area so that its borders will be parallel to the sides of the photo and the cuts will go straight between the pixel borders.</p><p>Now Polycarpus keeps wondering how many ways there are to cut an area out of the photo so that it met the conditions given above. Help Polycarpus find this number.</p></div><div class="input-specification"><p>The first line of the input data contains three integers <span class="tex-span"><i>n</i>, <i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 500;1 ≤ <i>k</i> ≤ <i>nm</i></span>). Then follow <span class="tex-span"><i>n</i></span> lines, containing the description of the given photo as a sequence of lines. Each line contains <span class="tex-span"><i>m</i></span> characters '<span class="tex-font-style-tt">0</span>' or '<span class="tex-font-style-tt">1</span>'.</p></div><div class="output-specification"><p>Print the required number of areas on the given photo.</p></div>

## Input

<p>The first line of the input data contains three integers <span class="tex-span"><i>n</i>, <i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 500;1 ≤ <i>k</i> ≤ <i>nm</i></span>). Then follow <span class="tex-span"><i>n</i></span> lines, containing the description of the given photo as a sequence of lines. Each line contains <span class="tex-span"><i>m</i></span> characters '<span class="tex-font-style-tt">0</span>' or '<span class="tex-font-style-tt">1</span>'.</p>

## Output

<p>Print the required number of areas on the given photo.</p>





```input1
4 6 2
111000
111100
011011
000111

```




```input2
5 5 4
11111
11111
11111
11111
11111

```




```output1
6

```




```output2
9

```



## Note

<p>We'll number the rows and columns below starting from 1, the coordinates <span class="tex-span">(<i>p</i>, <i>q</i>)</span> will denote a cell in row <span class="tex-span"><i>p</i></span>, column <span class="tex-span"><i>q</i></span>.</p><p>In the first sample Polycarpus should cut out any area containing a rectangle whose opposite corners lie in cells <span class="tex-span">(1, 1)</span> and (<span class="tex-span">3, 4</span>). Only rectangles with opposite corners in <span class="tex-span">(1, 1)</span> and (<span class="tex-span"><i>x</i>, <i>y</i></span>), where <span class="tex-span"><i>x</i> ≥ 3</span> and <span class="tex-span"><i>y</i> ≥ 4</span> fit the conditions.</p><p>In the second sample any rectangle whose each side is no less than four, will do. The possible rectangle sizes are <span class="tex-span">4 × 4</span>, <span class="tex-span">4 × 5</span>, <span class="tex-span">5 × 4</span> and <span class="tex-span">5 × 5</span>. Such figures can be cut in 4 ways, 2 ways, 2 ways and 1 way correspondingly.</p><p>Please do not use the %lld specificator to read or write 64-bit integers in C++. It is preferred to use cin, cout streams or the %I64d specificator.</p>
