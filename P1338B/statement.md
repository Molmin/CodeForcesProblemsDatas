## Description

<div><p>You have unweighted tree of $n$ vertices. You have to assign a <span class="tex-font-style-bf">positive</span> weight to each edge so that the following condition would hold:</p><ul> <li> For every two different leaves $v_{1}$ and $v_{2}$ of this tree, <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR</a> of weights of all edges on the simple path between $v_{1}$ and $v_{2}$ has to be equal to $0$. </li></ul><p>Note that you can put <span class="tex-font-style-bf">very large</span> positive integers (like $10^{(10^{10})}$).</p><p>It's guaranteed that such assignment always exists under given constraints. Now let's define $f$ as <span class="tex-font-style-bf">the number of distinct weights</span> in assignment.</p><center> <img class="tex-graphics" src="file://cXWoDzWU.png" style="max-width: 100.0%;max-height: 100.0%;"> In this example, assignment is valid, because bitwise XOR of all edge weights between every pair of leaves is $0$. $f$ value is $2$ here, because there are $2$ distinct edge weights($4$ and $5$).<p><img class="tex-graphics" src="file://WyOUnLAD.png" style="max-width: 100.0%;max-height: 100.0%;"> In this example, assignment is invalid, because bitwise XOR of all edge weights between vertex $1$ and vertex $6$ ($3, 4, 5, 4$) is not $0$. </p></center><p>What are the minimum and the maximum possible values of $f$ for the given tree? Find and print both.</p></div><div class="input-specification"><p>The first line contains integer $n$ ($3 \le n \le 10^{5}$)&nbsp;— the number of vertices in given tree.</p><p>The $i$-th of the next $n-1$ lines contains two integers $a_{i}$ and $b_{i}$ ($1 \le a_{i} \lt b_{i} \le n$)&nbsp;— it means there is an edge between $a_{i}$ and $b_{i}$. It is guaranteed that given graph forms tree of $n$ vertices.</p></div><div class="output-specification"><p>Print two integers&nbsp;— the minimum and maximum possible value of $f$ can be made from valid assignment of given tree. Note that it's always possible to make an assignment under given constraints.</p></div>

## Input

<p>The first line contains integer $n$ ($3 \le n \le 10^{5}$)&nbsp;— the number of vertices in given tree.</p><p>The $i$-th of the next $n-1$ lines contains two integers $a_{i}$ and $b_{i}$ ($1 \le a_{i} \lt b_{i} \le n$)&nbsp;— it means there is an edge between $a_{i}$ and $b_{i}$. It is guaranteed that given graph forms tree of $n$ vertices.</p>

## Output

<p>Print two integers&nbsp;— the minimum and maximum possible value of $f$ can be made from valid assignment of given tree. Note that it's always possible to make an assignment under given constraints.</p>





```input1
6
1 3
2 3
3 4
4 5
5 6
```




```input2
6
1 3
2 3
3 4
4 5
4 6
```




```input3
7
1 2
2 7
3 4
4 7
5 6
6 7
```




```output1
1 4
```




```output2
3 3
```




```output3
1 6
```



## Note

<p>In the first example, possible assignments for each minimum and maximum are described in picture below. Of course, there are multiple possible assignments for each minimum and maximum. </p><center> <img class="tex-graphics" src="file://bZrSnKZr.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second example, possible assignments for each minimum and maximum are described in picture below. The $f$ value of valid assignment of this tree is always $3$. </p><center> <img class="tex-graphics" src="file://DefF4Efz.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the third example, possible assignments for each minimum and maximum are described in picture below. Of course, there are multiple possible assignments for each minimum and maximum. </p><center> <img class="tex-graphics" src="file://miCaBSeu.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
