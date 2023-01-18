## Description

<div><p>Karlsson has recently discovered a huge stock of berry jam jars in the basement of the house. More specifically, there were $2n$ jars of strawberry and blueberry jam.</p><p>All the $2n$ jars are arranged in a row. The stairs to the basement are exactly in the middle of that row. So when Karlsson enters the basement, he sees exactly $n$ jars to his left and $n$ jars to his right.</p><p>For example, the basement might look like this:</p><center> <img class="tex-graphics" src="file://83w30sp8.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Being the starightforward man he is, he immediately starts eating the jam. In one minute he chooses to empty either the first non-empty jar to his left or the first non-empty jar to his right.</p><p>Finally, Karlsson decided that at the end the amount of full strawberry and blueberry jam jars should become the same.</p><p>For example, this might be the result:</p><center> <img class="tex-graphics" src="file://3tIkxWI2.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-style-it">He has eaten $1$ jar to his left and then $5$ jars to his right.</span> <span class="tex-font-style-it">There remained exactly $3$ full jars of both strawberry and blueberry jam.</span> </center><p>Jars are numbered from $1$ to $2n$ from left to right, so Karlsson initially stands between jars $n$ and $n+1$.</p><p>What is the minimum number of jars Karlsson is required to empty so that an equal number of full strawberry and blueberry jam jars is left?</p><p>Your program should answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 1000$) — the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$).</p><p>The second line of each test case contains $2n$ integers $a_1, a_2, \dots, a_{2n}$ ($1 \le a_i \le 2$) — $a_i=1$ means that the $i$-th jar from the left is a strawberry jam jar and $a_i=2$ means that it is a blueberry jam jar.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case print the answer to it — the minimum number of jars Karlsson is required to empty so that an equal number of full strawberry and blueberry jam jars is left.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 1000$) — the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$).</p><p>The second line of each test case contains $2n$ integers $a_1, a_2, \dots, a_{2n}$ ($1 \le a_i \le 2$) — $a_i=1$ means that the $i$-th jar from the left is a strawberry jam jar and $a_i=2$ means that it is a blueberry jam jar.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case print the answer to it — the minimum number of jars Karlsson is required to empty so that an equal number of full strawberry and blueberry jam jars is left.</p>





```input1
4
6
1 1 1 2 2 1 2 1 2 1 1 2
2
1 2 1 2
3
1 1 1 1 1 1
2
2 1 1 1
```




```output1
6
0
6
2
```



## Note

<p>The picture from the statement describes the first test case.</p><p>In the second test case the number of strawberry and blueberry jam jars is already equal.</p><p>In the third test case Karlsson is required to eat all $6$ jars so that there remain $0$ jars of both jams.</p><p>In the fourth test case Karlsson can empty either the second and the third jars or the third and the fourth one. The both scenarios will leave $1$ jar of both jams.</p>
