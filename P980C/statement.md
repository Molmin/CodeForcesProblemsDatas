## Description

<div><p>Professor Ibrahim has prepared the final homework for his algorithm’s class. He asked his students to implement the Posterization Image Filter.</p><p>Their algorithm will be tested on an array of integers, where the $i$-th integer represents the color of the $i$-th pixel in the image. The image is in black and white, therefore the color of each pixel will be an integer between 0 and 255 (inclusive).</p><p>To implement the filter, students are required to divide the black and white color range [0, 255] into groups of consecutive colors, and select one color in each group to be the group’s key. In order to preserve image details, the size of a group must not be greater than $k$, and each color should belong to exactly one group.</p><p>Finally, the students will replace the color of each pixel in the array with that color’s assigned group key.</p><p>To better understand the effect, here is an image of a basking turtle where the Posterization Filter was applied with increasing $k$ to the right. </p><center> <img class="tex-graphics" src="file://fvlVltzu.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>To make the process of checking the final answer easier, Professor Ibrahim wants students to divide the groups and assign the keys in a way that produces the lexicographically smallest possible array.</p></div><div class="input-specification"><p>The first line of input contains two integers $n$ and $k$ ($1 \leq n \leq 10^5$, $1 \leq k \leq 256$), the number of pixels in the image, and the maximum size of a group, respectively.</p><p>The second line contains $n$ integers $p_1, p_2, \dots, p_n$ ($0 \leq p_i \leq 255$), where $p_i$ is the color of the $i$-th pixel.</p></div><div class="output-specification"><p>Print $n$ space-separated integers; the lexicographically smallest possible array that represents the image after applying the Posterization filter.</p></div>

## Input

<p>The first line of input contains two integers $n$ and $k$ ($1 \leq n \leq 10^5$, $1 \leq k \leq 256$), the number of pixels in the image, and the maximum size of a group, respectively.</p><p>The second line contains $n$ integers $p_1, p_2, \dots, p_n$ ($0 \leq p_i \leq 255$), where $p_i$ is the color of the $i$-th pixel.</p>

## Output

<p>Print $n$ space-separated integers; the lexicographically smallest possible array that represents the image after applying the Posterization filter.</p>





```input1
4 3
2 14 3 4

```




```input2
5 2
0 2 1 255 254

```




```output1
0 12 3 3

```




```output2
0 1 1 254 254

```



## Note

<p>One possible way to group colors and assign keys for the first sample:</p><p>Color $2$ belongs to the group $[0,2]$, with group key $0$.</p><p>Color $14$ belongs to the group $[12,14]$, with group key $12$.</p><p>Colors $3$ and $4$ belong to group $[3, 5]$, with group key $3$.</p><p>Other groups won't affect the result so they are not listed here.</p>
