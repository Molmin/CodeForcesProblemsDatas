## Description

<div><p>You are given a $1$ by $n$ pixel image. The $i$-th pixel of the image has color $a_i$. For each color, the number of pixels of that color is <span class="tex-font-style-bf">at most</span> $20$.</p><p>You can perform the following operation, which works like the bucket tool in paint programs, on this image: </p><ul> <li> pick a color — an integer from $1$ to $n$; </li><li> choose a pixel in the image; </li><li> for all pixels connected to the selected pixel, change their colors to the selected color (two pixels of the same color are considered connected if all the pixels between them have the same color as those two pixels). </li></ul><p>Compute the minimum number of operations needed to make all the pixels in the image have the same color.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^3$).</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 3\cdot10^3$) — the number of pixels in the image.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$) — the colors of the pixels in the image.</p><p>Note: for each color, the number of pixels of that color is <span class="tex-font-style-bf">at most</span> $20$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3\cdot10^3$.</p></div><div class="output-specification"><p>For each test case, print one integer: the minimum number of operations needed to make all the pixels in the image have the same color.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^3$).</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 3\cdot10^3$) — the number of pixels in the image.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$) — the colors of the pixels in the image.</p><p>Note: for each color, the number of pixels of that color is <span class="tex-font-style-bf">at most</span> $20$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3\cdot10^3$.</p>

## Output

<p>For each test case, print one integer: the minimum number of operations needed to make all the pixels in the image have the same color.</p>





```input1
3
5
1 2 3 2 1
4
1 1 2 2
5
1 2 1 4 2
```




```output1
2
1
3
```



## Note

<p>In the first example, the optimal solution is to apply the operation on the third pixel changing its color to $2$ and then to apply the operation on any pixel that has color $2$ changing its color and the color of all pixels connected to it to $1$. The sequence of operations is then: $[1, 2, 3, 2, 1] \to [1, 2, 2, 2, 1] \to [1, 1, 1, 1, 1]$.</p><p>In the second example, we can either change the $1$s to $2$s in one operation or change the $2$s to $1$s also in one operation.</p><p>In the third example, one possible way to make all the pixels have the same color is to apply the operation on the first, third and the fourth pixel each time changing its color to $2$.</p>
