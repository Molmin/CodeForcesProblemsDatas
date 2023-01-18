## Description

<div><p>You came to the exhibition and one exhibit has drawn your attention. It consists of $n$ stacks of blocks, where the $i$-th stack consists of $a_i$ blocks resting on the surface.</p><p>The height of the exhibit is equal to $m$. Consequently, the number of blocks in each stack is less than or equal to $m$.</p><p>There is a camera on the ceiling that sees the top view of the blocks and a camera on the right wall that sees the side view of the blocks.</p><center><img class="tex-graphics" src="file://NOHF0p4l.png" style="max-width: 100.0%;max-height: 100.0%;"></center> <p>Find the maximum number of blocks you can remove such that the views for both the cameras would not change.</p><p>Note, that while originally all blocks are stacked on the floor, it is not required for them to stay connected to the floor after some blocks are removed. There is <span class="tex-font-style-bf">no gravity</span> in the whole exhibition, so no block would fall down, even if the block underneath is removed. It is not allowed to move blocks by hand either.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n \le 100\,000$, $1 \le m \le 10^9$)&nbsp;— the number of stacks and the height of the exhibit.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le m$)&nbsp;— the number of blocks in each stack from left to right.</p></div><div class="output-specification"><p>Print exactly one integer&nbsp;— the maximum number of blocks that can be removed.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n \le 100\,000$, $1 \le m \le 10^9$)&nbsp;— the number of stacks and the height of the exhibit.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le m$)&nbsp;— the number of blocks in each stack from left to right.</p>

## Output

<p>Print exactly one integer&nbsp;— the maximum number of blocks that can be removed.</p>





```input1
5 6
3 3 3 3 3

```




```input2
3 5
1 2 4

```




```input3
5 5
2 3 1 4 4

```




```input4
1 1000
548

```




```input5
3 3
3 1 1

```




```output1
10
```




```output2
3
```




```output3
9
```




```output4
0
```




```output5
1
```



## Note

<p>The following pictures illustrate the first example and its possible solution.</p><p>Blue cells indicate removed blocks. There are $10$ blue cells, so the answer is $10$.</p><center><img class="tex-graphics" src="file://d522vpuk.png" style="max-width: 100.0%;max-height: 100.0%;"></center>
