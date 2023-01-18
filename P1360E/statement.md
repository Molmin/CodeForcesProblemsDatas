## Description

<div><p>Polygon is not only the best platform for developing problems but also a square matrix with side $n$, initially filled with the character <span class="tex-font-style-tt">0</span>.</p><p>On the polygon, military training was held. The soldiers placed a cannon above each cell in the first row and a cannon to the left of each cell in the first column. Thus, exactly $2n$ cannons were placed.</p><center> <img class="tex-graphics" src="file://AxzWAVxD.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">Initial polygon for $n=4$.</span> </center><p>Cannons shoot character <span class="tex-font-style-tt">1</span>. At any moment of time, no more than one cannon is shooting. When a <span class="tex-font-style-tt">1</span> flies out of a cannon, it flies forward (in the direction of the shot) until it collides with a polygon border or another <span class="tex-font-style-tt">1</span>. After that, it takes the cell in which it was before the collision and remains there. Take a look at the examples for better understanding.</p><p>More formally: </p><ul> <li> if a cannon stands in the row $i$, to the left of the first column, and shoots with a <span class="tex-font-style-tt">1</span>, then the <span class="tex-font-style-tt">1</span> starts its flight from the cell ($i, 1$) and ends in some cell ($i, j$); </li><li> if a cannon stands in the column $j$, above the first row, and shoots with a <span class="tex-font-style-tt">1</span>, then the <span class="tex-font-style-tt">1</span> starts its flight from the cell ($1, j$) and ends in some cell ($i, j$). </li></ul><p>For example, consider the following sequence of shots:</p><center> <img class="tex-graphics" src="file://RQlP2MiD.png" style="max-width: 100.0%;max-height: 100.0%;"> <p> <span class="tex-font-size-small">1. Shoot the cannon in the row $2$. &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2. Shoot the cannon in the row $2$. &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 3. Shoot the cannon in column $3$.</span> </p></center><p>You have a report from the military training on your desk. This report is a square matrix with side length $n$ consisting of <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>. You wonder if the training actually happened. In other words, is there a sequence of shots such that, after the training, you get the given matrix?</p><p>Each cannon can make an arbitrary number of shots. Before the training, each cell of the polygon contains <span class="tex-font-style-tt">0</span>.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases. Then $t$ test cases follow.</p><p>Each test case starts with a line containing an integer $n$ ($1 \le n \le 50$)&nbsp;— the size of the polygon.</p><p>This is followed by $n$ lines of length $n$, consisting of <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>&nbsp;— the polygon matrix after the training.</p><p>The total area of the matrices in all test cases in one test does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case print:</p><ul> <li> <span class="tex-font-style-tt">YES</span> if there is a sequence of shots leading to a given matrix; </li><li> <span class="tex-font-style-tt">NO</span> if such a sequence does not exist. </li></ul><p>The letters in the words <span class="tex-font-style-tt">YES</span> and <span class="tex-font-style-tt">NO</span> can be printed in any case.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases. Then $t$ test cases follow.</p><p>Each test case starts with a line containing an integer $n$ ($1 \le n \le 50$)&nbsp;— the size of the polygon.</p><p>This is followed by $n$ lines of length $n$, consisting of <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>&nbsp;— the polygon matrix after the training.</p><p>The total area of the matrices in all test cases in one test does not exceed $10^5$.</p>

## Output

<p>For each test case print:</p><ul> <li> <span class="tex-font-style-tt">YES</span> if there is a sequence of shots leading to a given matrix; </li><li> <span class="tex-font-style-tt">NO</span> if such a sequence does not exist. </li></ul><p>The letters in the words <span class="tex-font-style-tt">YES</span> and <span class="tex-font-style-tt">NO</span> can be printed in any case.</p>





```input1
5
4
0010
0011
0000
0000
2
10
01
2
00
00
4
0101
1111
0101
0111
4
0100
1110
0101
0111
```




```output1
YES
NO
YES
YES
NO
```



## Note

<p>The first test case was explained in the statement.</p><p>The answer to the second test case is <span class="tex-font-style-tt">NO</span>, since a <span class="tex-font-style-tt">1</span> in a cell ($1, 1$) flying out of any cannon would continue its flight further.</p>
