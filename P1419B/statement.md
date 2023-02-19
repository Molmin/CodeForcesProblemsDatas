## Description

<div><p>Jett is tired after destroying the town and she wants to have a rest. She likes high places, that's why for having a rest she wants to get high and she decided to craft staircases.</p><p>A staircase is a squared figure that consists of square cells. Each staircase consists of an arbitrary number of stairs. If a staircase has $n$ stairs, then it is made of $n$ columns, the first column is $1$ cell high, the second column is $2$ cells high, $\ldots$, the $n$-th column if $n$ cells high. The lowest cells of all stairs must be in the same row.</p><p>A staircase with $n$ stairs is called nice, if it may be covered by $n$ <span class="tex-font-style-bf">disjoint</span> squares made of cells. All squares should fully consist of cells of a staircase.</p><center> This is how a nice covered staircase with $7$ stairs looks like: <img class="tex-graphics" src="file://7tE0YPYE.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Find out the maximal number of <span class="tex-font-style-bf">different</span> nice staircases, that can be built, using no more than $x$ cells, <span class="tex-font-style-bf">in total</span>. No cell can be used more than once.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ $(1 \le t \le 1000)$ &nbsp;— the number of test cases.</p><p>The description of each test case contains a single integer $x$ $(1 \le x \le 10^{18})$ &nbsp;— the number of cells for building staircases.</p></div><div class="output-specification"><p>For each test case output a single integer &nbsp;— the number of different nice staircases, that can be built, using not more than $x$ cells, in total.</p></div>

## Input

<p>The first line contains a single integer $t$ $(1 \le t \le 1000)$ &nbsp;— the number of test cases.</p><p>The description of each test case contains a single integer $x$ $(1 \le x \le 10^{18})$ &nbsp;— the number of cells for building staircases.</p>

## Output

<p>For each test case output a single integer &nbsp;— the number of different nice staircases, that can be built, using not more than $x$ cells, in total.</p>





```input1
4
1
8
6
1000000000000000000
```




```output1
1
2
1
30
```



## Note

<p>In the first test case, it is possible to build only one staircase, that consists of $1$ stair. It's nice. That's why the answer is $1$.</p><p>In the second test case, it is possible to build two different nice staircases: one consists of $1$ stair, and another consists of $3$ stairs. This will cost $7$ cells. In this case, there is one cell left, but it is not possible to use it for building any nice staircases, that have not been built yet. That's why the answer is $2$.</p><p>In the third test case, it is possible to build only one of two nice staircases: with $1$ stair or with $3$ stairs. In the first case, there will be $5$ cells left, that may be used only to build a staircase with $2$ stairs. This staircase is not nice, and Jett only builds nice staircases. That's why in this case the answer is $1$. If Jett builds a staircase with $3$ stairs, then there are no more cells left, so the answer is $1$ again.</p>
