## Description

<div><p>Tokitsukaze is arranging a meeting. There are $n$ rows and $m$ columns of seats in the meeting hall.</p><p>There are exactly $n \cdot m$ students attending the meeting, including several naughty students and several serious students. The students are numerated from $1$ to $n\cdot m$. The students will enter the meeting hall in order. When the $i$-th student enters the meeting hall, he will sit in the $1$-st column of the $1$-st row, and the students who are already seated will move back one seat. Specifically, the student sitting in the $j$-th ($1\leq j \leq m-1$) column of the $i$-th row will move to the $(j+1)$-th column of the $i$-th row, and the student sitting in $m$-th column of the $i$-th row will move to the $1$-st column of the $(i+1)$-th row.</p><p>For example, there is a meeting hall with $2$ rows and $2$ columns of seats shown as below:</p><center> <img class="tex-graphics" src="file://vQ3TooGg.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>There will be $4$ students entering the meeting hall in order, represented as a binary string "<span class="tex-font-style-tt">1100</span>", of which '<span class="tex-font-style-tt">0</span>' represents naughty students and '<span class="tex-font-style-tt">1</span>' represents serious students. The changes of seats in the meeting hall are as follows:</p><center> <img class="tex-graphics" src="file://qu3K1Jlj.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Denote a row or a column good if and only if there is at least one serious student in this row or column. Please predict the number of good rows and columns just after the $i$-th student enters the meeting hall, for all $i$.</p></div><div class="input-specification"><p>The first contains a single positive integer $t$ ($1 \leq t \leq 10\,000$)&nbsp;— the number of test cases.</p><p>For each test case, the first line contains two integers $n$, $m$ ($1 \leq n,m \leq 10^6$; $1 \leq n \cdot m \leq 10^6$), denoting there are $n$ rows and $m$ columns of seats in the meeting hall.</p><p>The second line contains a binary string $s$ of length $n \cdot m$, consisting only of zeros and ones. If $s_i$ equal to '<span class="tex-font-style-tt">0</span>' represents the $i$-th student is a naughty student, and $s_i$ equal to '<span class="tex-font-style-tt">1</span>' represents the $i$-th student is a serious student.</p><p>It is guaranteed that the sum of $n \cdot m$ over all test cases does not exceed $10^6$.</p></div><div class="output-specification"><p>For each test case, print a single line with $n \cdot m$ integers&nbsp;— the number of good rows and columns just after the $i$-th student enters the meeting hall.</p></div>

## Input

<p>The first contains a single positive integer $t$ ($1 \leq t \leq 10\,000$)&nbsp;— the number of test cases.</p><p>For each test case, the first line contains two integers $n$, $m$ ($1 \leq n,m \leq 10^6$; $1 \leq n \cdot m \leq 10^6$), denoting there are $n$ rows and $m$ columns of seats in the meeting hall.</p><p>The second line contains a binary string $s$ of length $n \cdot m$, consisting only of zeros and ones. If $s_i$ equal to '<span class="tex-font-style-tt">0</span>' represents the $i$-th student is a naughty student, and $s_i$ equal to '<span class="tex-font-style-tt">1</span>' represents the $i$-th student is a serious student.</p><p>It is guaranteed that the sum of $n \cdot m$ over all test cases does not exceed $10^6$.</p>

## Output

<p>For each test case, print a single line with $n \cdot m$ integers&nbsp;— the number of good rows and columns just after the $i$-th student enters the meeting hall.</p>





```input1
3
2 2
1100
4 2
11001101
2 4
11001101
```




```output1
2 3 4 3
2 3 4 3 5 4 6 5
2 3 3 3 4 4 4 5
```



## Note

<p>The first test case is shown in the statement.</p><p>After the $1$-st student enters the meeting hall, there are $2$ good rows and columns: the $1$-st row and the $1$-st column.</p><p>After the $2$-nd student enters the meeting hall, there are $3$ good rows and columns: the $1$-st row, the $1$-st column and the $2$-nd column.</p><p>After the $3$-rd student enters the meeting hall, the $4$ rows and columns are all good.</p><p>After the $4$-th student enters the meeting hall, there are $3$ good rows and columns: the $2$-nd row, the $1$-st column and the $2$-nd column.</p>
