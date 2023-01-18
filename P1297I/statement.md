## Description

<div><p>Recently, Polycarp has invented a new mobile game with falling blocks.</p><p>In the game, $n$ blocks are falling down, one at a time, towards a flat surface with length $d$ units. Each block can be represented as a rectangle with coordinates from $l_i$ to $r_i$ and unit height, dropped downwards from very high up. A block falls until it comes in contact with the flat surface or any other block. Let's define that block $a$ covers block $b$ if $l_a \le l_b \le r_b \le r_a$. </p><p>Consider what happens when a new block $i$ falls. If the new (upper) block $i$ comes in contact with <span class="tex-font-style-bf">any</span> block $j$ such that block $i$ <span class="tex-font-style-bf">does not</span> cover block $j$, block $i$ will stick to block $j$, and <span class="tex-font-style-bf">no blocks will disappear</span>. Otherwise, all blocks that block $i$ covers and is in contact with will be vaporized, and block $i$ will continue falling with the ability to vaporize lower blocks.</p><p>For example, consider what happens when three blocks $(1,2)$, $(2,3)$ and $(1,3)$ fall, in that order. The first block will stick to the flat surface. Then, the second block will stick to the first block. Finally, the third block will vaporize the second block, keep falling, vaporize the first block, and stick to the flat surface.</p><center> <img class="tex-graphics" height="113px" src="file://uDQm5GJS.png" style="max-width: 100.0%;max-height: 100.0%;" width="1134px">   <span class="tex-font-size-small">Here is a graphic for the first example.</span> </center><p>After each block falls, help Polycarp determine how many blocks will remain!</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $d$ ($1 \le n, d \le 10^5$) &nbsp;— the number of falling blocks and the length of the flat surface.</p><p>The $i$-th of the following $n$ lines contains integers $l_i$ and $r_i$ ($1 \le l_i \le r_i \le d$) &nbsp;— the coordinates of the $i$-th block. </p></div><div class="output-specification"><p>Output $n$ integers. The $i$-th integer should be the number of blocks that will be left after the $i$-th block falls.</p></div>

## Input

<p>The first line contains two integers $n$ and $d$ ($1 \le n, d \le 10^5$) &nbsp;— the number of falling blocks and the length of the flat surface.</p><p>The $i$-th of the following $n$ lines contains integers $l_i$ and $r_i$ ($1 \le l_i \le r_i \le d$) &nbsp;— the coordinates of the $i$-th block. </p>

## Output

<p>Output $n$ integers. The $i$-th integer should be the number of blocks that will be left after the $i$-th block falls.</p>





```input1
3 3
1 2
2 3
1 3
```




```input2
8 6
1 2
3 3
2 3
1 3
2 4
3 6
1 5
1 5
```




```output1
1
2
1
```




```output2
1
2
3
1
2
3
4
4
```



## Note

<p>The first example is explained above.</p><p>In the second example, this is what happens after each block falls: </p><ul> <li> Block $1$ will stick to the flat surface. </li><li> Block $2$ will stick to the flat surface. </li><li> Block $3$ will stick to blocks $1$ and $2$. Note that block $3$ will not vaporize block $2$ because it does not cover block $1$ and is in contact with it. </li><li> Block $4$ will vaporize all the blocks and stick to the flat surface. </li><li> Block $5$ will stick to block $4$ </li><li> Block $6$ will stick to block $5$. </li><li> Block $7$ will stick to block $6$. Note that no blocks are vaporized because although block $7$ covers block $4$ and block $5$, they never come in contact. </li><li> Block $8$ vaporizes block $7$ and sticks to block $6$. </li></ul>
