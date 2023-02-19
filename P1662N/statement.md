## Description

<div><p>Today, like every year at SWERC, the $n^2$ contestants have gathered outside the venue to take a drone photo. Jennifer, the social media manager for the event, has arranged them into an $n\times n$ square. Being very good at her job, she knows that the contestant standing on the intersection of the $i$-th row with the $j$-th column is $a_{i,j}$ years old. Coincidentally, she notices that no two contestants have the same age, and that everyone is between $1$ and $n^2$ years old.</p><p>Jennifer is planning to have some contestants hold a banner with the ICPC logo parallel to the ground, so that it is clearly visible in the aerial picture. Here are the steps that she is going to follow in order to take the perfect SWERC drone photo.</p><ul> <li> First of all, Jennifer is going to select four contestants standing on the vertices of an axis-aligned rectangle. </li><li> Then, she will have the two younger contestants hold one of the poles, while the two older contestants will hold the other pole. </li><li> Finally, she will unfold the banner, using the poles to support its two ends. Obviously, this can only be done if the two poles are parallel and <span class="tex-font-style-bf">do not cross</span>, as shown in the pictures below. </li></ul> <center> <img class="tex-graphics" src="file://6qjo5MzO.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Being very indecisive, Jennifer would like to try out all possible arrangements for the banner, but she is worried that this may cause the contestants to be late for the competition. How many different ways are there to choose the four contestants holding the poles in order to take a perfect photo? Two choices are considered different if at least one contestant is included in one but not the other.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2\le n \le 1500$).</p><p>The next $n$ lines describe the ages of the contestants. Specifically, the $i$-th line contains the integers $a_{i,1},a_{i,2},\ldots,a_{i,n}$ ($1\le a_{i,j}\le n^2$).</p><p>It is guaranteed that $a_{i,j}\neq a_{k,l}$ if $i\neq k$ or $j\neq l$.</p></div><div class="output-specification"><p>Print the number of ways for Jennifer to choose the four contestants holding the poles.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2\le n \le 1500$).</p><p>The next $n$ lines describe the ages of the contestants. Specifically, the $i$-th line contains the integers $a_{i,1},a_{i,2},\ldots,a_{i,n}$ ($1\le a_{i,j}\le n^2$).</p><p>It is guaranteed that $a_{i,j}\neq a_{k,l}$ if $i\neq k$ or $j\neq l$.</p>

## Output

<p>Print the number of ways for Jennifer to choose the four contestants holding the poles.</p>





```input1
2
1 3
4 2
```




```input2
2
3 2
4 1
```




```input3
3
9 2 4
1 5 3
7 8 6
```




```output1
0
```




```output2
1
```




```output3
6
```



## Note

<p>In the <span class="tex-font-style-bf">first sample</span>, there are $4$ contestants, arranged as follows. </p><center> <img class="tex-graphics" src="file://7iInROW4.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>There is only one way to choose four contestants, with one pole held by contestants aged $1$ and $2$ and the other one by contestants aged $3$ and $4$. But then, as we can see in the picture, the poles cross. </p><center> <img class="tex-graphics" src="file://ZK8pevlY.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Since there is no valid way to choose four contestants, the answer is $0$.</p><p>In the <span class="tex-font-style-bf">second sample</span>, the $4$ contestants are arranged as follows. </p><center> <img class="tex-graphics" src="file://WcklRNZ9.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Once again, there is only one way to choose four contestants, but this time the poles don't cross. </p><center> <img class="tex-graphics" src="file://YhgCkhsK.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Therefore, the answer is $1$.</p><p>In the <span class="tex-font-style-bf">third sample</span>, the $9$ contestants are arranged as follows. </p><center> <img class="tex-graphics" src="file://XY5lrn0q.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>There are $6$ ways of choosing four contestants so that the poles don't cross, as shown in the following pictures. </p><center> <img class="tex-graphics" src="file://sby21eab.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
