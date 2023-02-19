## Description

<div><p>Petya is a math teacher. $n$ of his students has written a test consisting of $m$ questions. For each student, it is known which questions he has answered correctly and which he has not.</p><p>If the student answers the $j$-th question correctly, he gets $p_j$ points (otherwise, he gets $0$ points). Moreover, the points for the questions are distributed in such a way that the array $p$ is a permutation of numbers from $1$ to $m$.</p><p>For the $i$-th student, Petya knows that he expects to get $x_i$ points for the test. Petya wonders how unexpected the results could be. Petya believes that the <span class="tex-font-style-it">surprise value</span> of the results for students is equal to $\sum\limits_{i=1}^{n} |x_i - r_i|$, where $r_i$ is the number of points that the $i$-th student has got for the test.</p><p>Your task is to help Petya find such a permutation $p$ for which the <span class="tex-font-style-it">surprise value</span> of the results is maximum possible. If there are multiple answers, print any of them.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n \le 10$; $1 \le m \le 10^4$)&nbsp;— the number of students and the number of questions, respectively.</p><p>The second line contains $n$ integers $x_1, x_2, \dots, x_n$ ($0 \le x_i \le \frac{m(m+1)}{2}$), where $x_i$ is the number of points that the $i$-th student expects to get.</p><p>This is followed by $n$ lines, the $i$-th line contains the string $s_i$ ($|s_i| = m; s_{i, j} \in \{0, 1\}$), where $s_{i, j}$ is $1$ if the $i$-th student has answered the $j$-th question correctly, and $0$ otherwise.</p><p>The sum of $m$ for all test cases does not exceed $10^4$.</p></div><div class="output-specification"><p>For each test case, print $m$ integers&nbsp;— a permutation $p$ for which the <span class="tex-font-style-it">surprise value</span> of the results is maximum possible. If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n \le 10$; $1 \le m \le 10^4$)&nbsp;— the number of students and the number of questions, respectively.</p><p>The second line contains $n$ integers $x_1, x_2, \dots, x_n$ ($0 \le x_i \le \frac{m(m+1)}{2}$), where $x_i$ is the number of points that the $i$-th student expects to get.</p><p>This is followed by $n$ lines, the $i$-th line contains the string $s_i$ ($|s_i| = m; s_{i, j} \in \{0, 1\}$), where $s_{i, j}$ is $1$ if the $i$-th student has answered the $j$-th question correctly, and $0$ otherwise.</p><p>The sum of $m$ for all test cases does not exceed $10^4$.</p>

## Output

<p>For each test case, print $m$ integers&nbsp;— a permutation $p$ for which the <span class="tex-font-style-it">surprise value</span> of the results is maximum possible. If there are multiple answers, print any of them.</p>





```input1
3
4 3
5 1 2 2
110
100
101
100
4 4
6 2 0 10
1001
0010
0110
0101
3 6
20 3 15
010110
000101
111111
```




```output1
3 1 2 
2 3 4 1 
3 1 4 5 2 6
```


