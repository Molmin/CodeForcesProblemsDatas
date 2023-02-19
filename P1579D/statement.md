## Description

<div><p>An important meeting is to be held and there are exactly $n$ people invited. At any moment, any two people can step back and talk in private. The same two people can talk several (as many as they want) times per meeting.</p><p>Each person has limited <span class="tex-font-style-it">sociability</span>. The sociability of the $i$-th person is a non-negative integer $a_i$. This means that after exactly $a_i$ talks this person leaves the meeting (and does not talk to anyone else anymore). If $a_i = 0$, the $i$-th person leaves the meeting immediately after it starts.</p><p>A meeting is considered most <span class="tex-font-style-it">productive</span> if the maximum possible number of talks took place during it.</p><p>You are given an array of sociability $a$, determine which people should talk to each other so that the total number of talks is as large as possible.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>The next $2t$ lines contain descriptions of the test cases.</p><p>The first line of each test case description contains an integer $n$ ($2 \le n \le 2 \cdot 10^5$)&nbsp;—the number of people in the meeting. The second line consists of $n$ space-separated integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 2 \cdot 10^5$)&nbsp;— the sociability parameters of all people. </p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$. It is also guaranteed that the sum of all $a_i$ (over all test cases and all $i$) does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>Print $t$ answers to all test cases.</p><p>On the first line of each answer print the number $k$&nbsp;— the maximum number of talks possible in a meeting.</p><p>On each of the next $k$ lines print two integers $i$ and $j$ ($1 \le i, j \le n$ and $i \neq j$)&nbsp;— the numbers of people who will have another talk.</p><p>If there are several possible answers, you may print any of them.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>The next $2t$ lines contain descriptions of the test cases.</p><p>The first line of each test case description contains an integer $n$ ($2 \le n \le 2 \cdot 10^5$)&nbsp;—the number of people in the meeting. The second line consists of $n$ space-separated integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 2 \cdot 10^5$)&nbsp;— the sociability parameters of all people. </p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$. It is also guaranteed that the sum of all $a_i$ (over all test cases and all $i$) does not exceed $2 \cdot 10^5$.</p>

## Output

<p>Print $t$ answers to all test cases.</p><p>On the first line of each answer print the number $k$&nbsp;— the maximum number of talks possible in a meeting.</p><p>On each of the next $k$ lines print two integers $i$ and $j$ ($1 \le i, j \le n$ and $i \neq j$)&nbsp;— the numbers of people who will have another talk.</p><p>If there are several possible answers, you may print any of them.</p>





```input1
8
2
2 3
3
1 2 3
4
1 2 3 4
3
0 0 2
2
6 2
3
0 0 2
5
8 2 0 1 1
5
0 1 0 0 6
```




```output1
2
1 2
1 2
3
1 3
2 3
2 3
5
1 3
2 4
2 4
3 4
3 4
0
2
1 2
1 2
0
4
1 2
1 5
1 4
1 2
1
5 2
```


