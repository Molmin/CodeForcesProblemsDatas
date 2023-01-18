## Description

<div><p>As a professional private tutor, Kuroni has to gather statistics of an exam. Kuroni has appointed you to complete this important task. You must not disappoint him.</p><p>The exam consists of $n$ questions, and $m$ students have taken the exam. Each question was worth $1$ point. Question $i$ was solved by at least $l_i$ and at most $r_i$ students. Additionally, you know that the total score of all students is $t$.</p><p>Furthermore, you took a glance at the final ranklist of the quiz. The students were ranked from $1$ to $m$, where rank $1$ has the highest score and rank $m$ has the lowest score. Ties were broken arbitrarily.</p><p>You know that the student at rank $p_i$ had a score of $s_i$ for $1 \le i \le q$.</p><p>You wonder if there could have been a huge tie for first place. Help Kuroni determine the maximum number of students who could have gotten as many points as the student with rank $1$, and the maximum possible score for rank $1$ achieving this maximum number of students.</p></div><div class="input-specification"><p>The first line of input contains two integers ($1 \le n, m \le 10^{5}$), denoting the number of questions of the exam and the number of students respectively.</p><p>The next $n$ lines contain two integers each, with the $i$-th line containing $l_{i}$ and $r_{i}$ ($0 \le l_{i} \le r_{i} \le m$).</p><p>The next line contains a single integer $q$ ($0 \le q \le m$). </p><p>The next $q$ lines contain two integers each, denoting $p_{i}$ and $s_{i}$ ($1 \le p_{i} \le m$, $0 \le s_{i} \le n$). It is guaranteed that all $p_{i}$ are distinct and if $p_{i} \le p_{j}$, then $s_{i} \ge s_{j}$.</p><p>The last line contains a single integer $t$ ($0 \le t \le nm$), denoting the total score of all students.</p></div><div class="output-specification"><p>Output two integers: the maximum number of students who could have gotten as many points as the student with rank $1$, and the maximum possible score for rank $1$ achieving this maximum number of students. If there is no valid arrangement that fits the given data, output $-1$ $-1$.</p></div>

## Input

<p>The first line of input contains two integers ($1 \le n, m \le 10^{5}$), denoting the number of questions of the exam and the number of students respectively.</p><p>The next $n$ lines contain two integers each, with the $i$-th line containing $l_{i}$ and $r_{i}$ ($0 \le l_{i} \le r_{i} \le m$).</p><p>The next line contains a single integer $q$ ($0 \le q \le m$). </p><p>The next $q$ lines contain two integers each, denoting $p_{i}$ and $s_{i}$ ($1 \le p_{i} \le m$, $0 \le s_{i} \le n$). It is guaranteed that all $p_{i}$ are distinct and if $p_{i} \le p_{j}$, then $s_{i} \ge s_{j}$.</p><p>The last line contains a single integer $t$ ($0 \le t \le nm$), denoting the total score of all students.</p>

## Output

<p>Output two integers: the maximum number of students who could have gotten as many points as the student with rank $1$, and the maximum possible score for rank $1$ achieving this maximum number of students. If there is no valid arrangement that fits the given data, output $-1$ $-1$.</p>





```input1
5 4
2 4
2 3
1 1
0 1
0 0
1
4 1
7
```




```input2
5 6
0 6
0 6
2 5
6 6
4 6
1
3 3
30
```




```output1
3 2
```




```output2
-1 -1
```



## Note

<p>For the first sample, here is one possible arrangement that fits the data:</p><p>Students $1$ and $2$ both solved problems $1$ and $2$.</p><p>Student $3$ solved problems $2$ and $3$.</p><p>Student $4$ solved problem $4$.</p><p>The total score of all students is $T = 7$. Note that the scores of the students are $2$, $2$, $2$ and $1$ respectively, which satisfies the condition that the student at rank $4$ gets exactly $1$ point. Finally, $3$ students tied for first with a maximum score of $2$, and it can be proven that we cannot do better with any other arrangement.</p>
