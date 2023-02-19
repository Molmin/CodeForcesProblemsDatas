## Description

<div><p>Leo Jr. draws pictures in his notebook with checkered sheets (that is, each sheet has a regular square grid printed on it). We can assume that the sheets are infinitely large in any direction.</p><p>To draw a picture, Leo Jr. colors some of the cells on a sheet gray. He considers the resulting picture <span class="tex-font-style-it">beautiful</span> if the following conditions are satisfied:</p><ul><li> The picture is <span class="tex-font-style-bf">connected</span>, that is, it is possible to get from any gray cell to any other by following a chain of gray cells, with each pair of adjacent cells in the path being neighbours (that is, sharing a side).</li><li> Each gray cell has an <span class="tex-font-style-bf">even number of gray neighbours</span>.</li><li> There are <span class="tex-font-style-bf">exactly $n$ gray cells with all gray neighbours</span>. The number of other gray cells can be arbitrary <span class="tex-font-style-it">(but reasonable, so that they can all be listed)</span>.</li></ul><p>Leo Jr. is now struggling to draw a beautiful picture with a particular choice of $n$. Help him, and provide any example of a beautiful picture.</p><p>To output cell coordinates in your answer, assume that the sheet is provided with a Cartesian coordinate system such that one of the cells is chosen to be the origin $(0, 0)$, axes $0x$ and $0y$ are orthogonal and parallel to grid lines, and a unit step along any axis in any direction takes you to a neighbouring cell.</p></div><div class="input-specification"><p>The only line contains a single integer $n$ ($1 \leq n \leq 500$)&nbsp;— the number of gray cells with all gray neighbours in a beautiful picture.</p></div><div class="output-specification"><p>In the first line, print a single integer $k$&nbsp;— the number of gray cells in your picture. For technical reasons, $k$ should not exceed $5 \cdot 10^5$.</p><p>Each of the following $k$ lines should contain two integers&nbsp;— coordinates of a gray cell in your picture. All listed cells should be distinct, and the picture should satisdfy all the properties listed above. All coordinates should not exceed $10^9$ by absolute value.</p><p>One can show that there exists an answer satisfying all requirements with a small enough $k$.</p></div>

## Input

<p>The only line contains a single integer $n$ ($1 \leq n \leq 500$)&nbsp;— the number of gray cells with all gray neighbours in a beautiful picture.</p>

## Output

<p>In the first line, print a single integer $k$&nbsp;— the number of gray cells in your picture. For technical reasons, $k$ should not exceed $5 \cdot 10^5$.</p><p>Each of the following $k$ lines should contain two integers&nbsp;— coordinates of a gray cell in your picture. All listed cells should be distinct, and the picture should satisdfy all the properties listed above. All coordinates should not exceed $10^9$ by absolute value.</p><p>One can show that there exists an answer satisfying all requirements with a small enough $k$.</p>





```input1
4
```




```output1
12
1 0
2 0
0 1
1 1
2 1
3 1
0 2
1 2
2 2
3 2
1 3
2 3
```



## Note

<p>The answer for the sample is pictured below:</p><center> <img class="tex-graphics" src="file://2qeXMnnf.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
