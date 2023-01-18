## Description

<div><p>You have a given picture with size $w \times h$. Determine if the given picture has a single "<span class="tex-font-style-tt">+</span>" shape or not. A "<span class="tex-font-style-tt">+</span>" shape is described below:</p><ul> <li> A "<span class="tex-font-style-tt">+</span>" shape has one center nonempty cell. </li><li> There should be some (at least one) consecutive non-empty cells in each direction (left, right, up, down) from the center. In other words, there should be a ray in each direction. </li><li> All other cells are empty. </li></ul><p>Find out if the given picture has single "<span class="tex-font-style-tt">+</span>" shape.</p></div><div class="input-specification"><p>The first line contains two integers $h$ and $w$ ($1 \le h$, $w \le 500$)&nbsp;— the height and width of the picture.</p><p>The $i$-th of the next $h$ lines contains string $s_{i}$ of length $w$ consisting "<span class="tex-font-style-tt">.</span>" and "<span class="tex-font-style-tt">*</span>" where "<span class="tex-font-style-tt">.</span>" denotes the empty space and "<span class="tex-font-style-tt">*</span>" denotes the non-empty space.</p></div><div class="output-specification"><p>If the given picture satisfies all conditions, print "<span class="tex-font-style-tt">YES</span>". Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p><p>You can output each letter in any case (upper or lower).</p></div>

## Input

<p>The first line contains two integers $h$ and $w$ ($1 \le h$, $w \le 500$)&nbsp;— the height and width of the picture.</p><p>The $i$-th of the next $h$ lines contains string $s_{i}$ of length $w$ consisting "<span class="tex-font-style-tt">.</span>" and "<span class="tex-font-style-tt">*</span>" where "<span class="tex-font-style-tt">.</span>" denotes the empty space and "<span class="tex-font-style-tt">*</span>" denotes the non-empty space.</p>

## Output

<p>If the given picture satisfies all conditions, print "<span class="tex-font-style-tt">YES</span>". Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p><p>You can output each letter in any case (upper or lower).</p>





```input1
5 6
......
..*...
.****.
..*...
..*...
```




```input2
3 5
..*..
****.
.*...
```




```input3
7 7
.......
...*...
..****.
...*...
...*...
.......
.*.....
```




```input4
5 6
..**..
..**..
******
..**..
..**..
```




```input5
3 7
.*...*.
***.***
.*...*.
```




```input6
5 10
..........
..*.......
.*.******.
..*.......
..........
```




```output1
YES
```




```output2
NO
```




```output3
NO
```




```output4
NO
```




```output5
NO
```




```output6
NO
```



## Note

<p>In the first example, the given picture contains one "<span class="tex-font-style-tt">+</span>".</p><p>In the second example, two vertical branches are located in a different column.</p><p>In the third example, there is a dot outside of the shape.</p><p>In the fourth example, the width of the two vertical branches is $2$.</p><p>In the fifth example, there are two shapes.</p><p>In the sixth example, there is an empty space inside of the shape.</p>
