## Description

<div><p>Inaka has a disc, the circumference of which is $n$ units. The circumference is equally divided by $n$ points numbered clockwise from $1$ to $n$, such that points $i$ and $i + 1$ ($1 \leq i &lt; n$) are adjacent, and so are points $n$ and $1$.</p><p>There are $m$ straight segments on the disc, the endpoints of which are all among the aforementioned $n$ points.</p><p>Inaka wants to know if her image is <span class="tex-font-style-it">rotationally symmetrical</span>, i.e. if there is an integer $k$ ($1 \leq k &lt; n$), such that if all segments are rotated clockwise around the center of the circle by $k$ units, the new image will be the same as the original one.</p></div><div class="input-specification"><p>The first line contains two space-separated integers $n$ and $m$ ($2 \leq n \leq 100\,000$, $1 \leq m \leq 200\,000$)&nbsp;— the number of points and the number of segments, respectively.</p><p>The $i$-th of the following $m$ lines contains two space-separated integers $a_i$ and $b_i$ ($1 \leq a_i, b_i \leq n$, $a_i \neq b_i$) that describe a segment connecting points $a_i$ and $b_i$.</p><p>It is guaranteed that no segments coincide.</p></div><div class="output-specification"><p>Output one line&nbsp;— "<span class="tex-font-style-tt">Yes</span>" if the image is rotationally symmetrical, and "<span class="tex-font-style-tt">No</span>" otherwise (both excluding quotation marks).</p><p>You can output each letter in any case (upper or lower).</p></div>

## Input

<p>The first line contains two space-separated integers $n$ and $m$ ($2 \leq n \leq 100\,000$, $1 \leq m \leq 200\,000$)&nbsp;— the number of points and the number of segments, respectively.</p><p>The $i$-th of the following $m$ lines contains two space-separated integers $a_i$ and $b_i$ ($1 \leq a_i, b_i \leq n$, $a_i \neq b_i$) that describe a segment connecting points $a_i$ and $b_i$.</p><p>It is guaranteed that no segments coincide.</p>

## Output

<p>Output one line&nbsp;— "<span class="tex-font-style-tt">Yes</span>" if the image is rotationally symmetrical, and "<span class="tex-font-style-tt">No</span>" otherwise (both excluding quotation marks).</p><p>You can output each letter in any case (upper or lower).</p>





```input1
12 6
1 3
3 7
5 7
7 11
9 11
11 3
```




```input2
9 6
4 5
5 6
7 8
8 9
1 2
2 3
```




```input3
10 3
1 2
3 2
7 2
```




```input4
10 2
1 6
2 7
```




```output1
Yes
```




```output2
Yes
```




```output3
No
```




```output4
Yes
```



## Note

<p>The first two examples are illustrated below. Both images become the same as their respective original ones after a clockwise rotation of $120$ degrees around the center.</p><center> <img class="tex-graphics" src="file://D0WVIMSe.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
