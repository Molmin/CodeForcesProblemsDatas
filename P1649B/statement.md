## Description

<div><p>Daniel is watching a football team playing a game during their training session. They want to improve their passing skills during that session.</p><p>The game involves $n$ players, making multiple passes towards each other. Unfortunately, since the balls were moving too fast, after the session Daniel is unable to know how many balls were involved during the game. The only thing he knows is the number of passes delivered by each player during all the session.</p><p>Find the minimum possible amount of balls that were involved in the game.</p></div><div class="input-specification"><p>There are several test cases in the input data. The first line contains a single integer $t$ ($1 \leq t \leq 5 \cdot 10^4$)&nbsp;— the number of test cases. This is followed by the test cases description.</p><p>The first line of each test case contains one integer $n$ ($2 \leq n \leq 10^5$)&nbsp;— the number of players.</p><p>The second line of the test case contains a sequence of integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i \leq 10^9$), where $a_i$ is the number of passes delivered by the $i$-th player.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $10^5$.</p></div><div class="output-specification"><p>For each test case print a single integer&nbsp;— the answer to the problem.</p></div>

## Input

<p>There are several test cases in the input data. The first line contains a single integer $t$ ($1 \leq t \leq 5 \cdot 10^4$)&nbsp;— the number of test cases. This is followed by the test cases description.</p><p>The first line of each test case contains one integer $n$ ($2 \leq n \leq 10^5$)&nbsp;— the number of players.</p><p>The second line of the test case contains a sequence of integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i \leq 10^9$), where $a_i$ is the number of passes delivered by the $i$-th player.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $10^5$.</p>

## Output

<p>For each test case print a single integer&nbsp;— the answer to the problem.</p>





```input1
4
4
2 3 3 2
3
1 5 2
2
0 0
4
1000000000 1000000000 1000000000 1000000000
```




```output1
1
2
0
1
```



## Note

<p>In the first test case, with the only ball, the game can go like this:</p><p>$2 \rightarrow 1 \rightarrow 3 \rightarrow 4 \rightarrow 1 \rightarrow 2 \rightarrow 3 \rightarrow 4 \rightarrow 2 \rightarrow 3 \rightarrow 2$.</p><p>In the second test case, there is no possible way to play the game with only one ball. One possible way to play with two balls:</p><p>$2 \rightarrow 1 \rightarrow 2 \rightarrow 3 \rightarrow 2 \rightarrow 1$.</p><p>$2 \rightarrow 3 \rightarrow 2 \rightarrow 1$</p><p>In the third example, there were no passes, so $0$ balls are possible.</p>
