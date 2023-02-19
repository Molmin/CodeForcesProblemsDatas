## Description

<div><p>A school has to decide on its team for an international quiz. There are $n$ students in the school. We can describe the students using an array $a$ where $a_i$ is the smartness of the $i$-th ($1 \le i \le n$) student. </p><p>There are $m$ topics $1, 2, 3, \ldots, m$ from which the quiz questions will be formed. The $i$-th student is considered proficient in a topic $T$ if $(a_i \bmod T) = 0$. Otherwise, he is a rookie in that topic. </p><p>We say that a team of students is collectively proficient in all the topics if for every topic there is a member of the team proficient in this topic.</p><p>Find a team that is collectively proficient in all the topics such that the maximum difference between the smartness of any two students in that team is <span class="tex-font-style-bf">minimized</span>. Output this difference.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains $n$ and $m$ ($1 \le n,m \le 10^5$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^5$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p><p>It is guaranteed that the sum of $m$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, print the answer on a new line. If there is no solution, output $-1$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains $n$ and $m$ ($1 \le n,m \le 10^5$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^5$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p><p>It is guaranteed that the sum of $m$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, print the answer on a new line. If there is no solution, output $-1$.</p>





```input1|2,3,6,7
3
2 4
3 7
4 2
3 7 2 9
5 7
6 4 3 5 7
```




```output1
-1
0
3
```



## Note

<p>In the first test case, we have participants with smartnesses $3$ and $7$, and $m = 4$. Thus, there is no student with smartness divisible by $2$. Since $2 \leq m$, there is no way to choose a team.</p><p>In the second test case, we can select the participant with smartness $2$ to be the only one on the team. This way the team will be collectively proficient in both topics $1$ and $2$.</p><p>In the third test case, consider the team with participants of smartnesses $4, 5, 6, 7$. This way the team will be collectively proficient in all topics $1, 2, \ldots, 7$.</p>
