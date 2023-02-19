## Description

<div><p><span class="tex-font-style-it">This is the easy version of the problem. The only difference from the hard version is that in this version all coordinates are <span class="tex-font-style-bf">even</span>.</span></p><p>There are $n$ fence-posts at distinct coordinates on a plane. It is guaranteed that no three fence posts lie on the same line.</p><p>There are an infinite number of cows on the plane, one at every point with integer coordinates.</p><p>Gregor is a member of the Illuminati, and wants to build a triangular fence, connecting $3$ distinct existing fence posts. A cow <span class="tex-font-style-bf">strictly</span> inside the fence is said to be <span class="tex-font-style-it">enclosed</span>. If there are an <span class="tex-font-style-bf">odd</span> number of enclosed cows and the area of the fence is an <span class="tex-font-style-bf">integer</span>, the fence is said to be <span class="tex-font-style-it">interesting</span>.</p><p>Find the number of interesting fences.</p></div><div class="input-specification"><p>The first line contains the integer $n$ ($3 \le n \le 6000$), the number of fence posts which Gregor can choose to form the vertices of a fence.</p><p>Each of the next $n$ line contains two integers $x$ and $y$ ($0 \le x,y \le 10^7$, $x$ and $y$ are <span class="tex-font-style-bf">even</span>), where $(x,y)$ is the coordinate of a fence post. All fence posts lie at distinct coordinates. No three fence posts are on the same line.</p></div><div class="output-specification"><p>Print a single integer, the number of interesting fences. Two fences are considered different if they are constructed with a different set of three fence posts.</p></div>

## Input

<p>The first line contains the integer $n$ ($3 \le n \le 6000$), the number of fence posts which Gregor can choose to form the vertices of a fence.</p><p>Each of the next $n$ line contains two integers $x$ and $y$ ($0 \le x,y \le 10^7$, $x$ and $y$ are <span class="tex-font-style-bf">even</span>), where $(x,y)$ is the coordinate of a fence post. All fence posts lie at distinct coordinates. No three fence posts are on the same line.</p>

## Output

<p>Print a single integer, the number of interesting fences. Two fences are considered different if they are constructed with a different set of three fence posts.</p>





```input1
3
0 0
2 0
0 4
```




```input2
5
0 0
2 16
30 14
4 6
2 10
```




```output1
1
```




```output2
3
```



## Note

<p>In the first example, there is only $1$ fence. That fence is interesting since its area is $4$ and there is $1$ enclosed cow, marked in red.</p><center> <img class="tex-graphics" src="file://KaDjSexG.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second example, there are $3$ interesting fences. </p><ul> <li> $(0,0)$ — $(30,14)$ — $(2,10)$ </li><li> $(2,16)$ — $(30,14)$ — $(2,10)$ </li><li> $(30,14)$ — $(4,6)$ — $(2,10)$ </li></ul>
