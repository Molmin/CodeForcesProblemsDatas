## Description

<div><p>Monocarp is a tutor of a group of $n$ students. He communicates with them using a conference in a popular messenger.</p><p>Today was a busy day for Monocarp — he was asked to forward a lot of posts and announcements to his group, that's why he had to write a very large number of messages in the conference. Monocarp knows the students in the group he is tutoring quite well, so he understands which message should each student read: Monocarp wants the student $i$ to read the message $m_i$.</p><p>Of course, no one's going to read all the messages in the conference. That's why Monocarp decided to pin some of them. Monocarp can pin any number of messages, and if he wants anyone to read some message, he should pin it — otherwise <span class="tex-font-style-bf">it will definitely be skipped by everyone</span>.</p><p>Unfortunately, even if a message is pinned, some students may skip it anyway. For each student $i$, Monocarp knows that they will read at most $k_i$ messages. Suppose Monocarp pins $t$ messages; if $t \le k_i$, then the $i$-th student will read all the pinned messages; but if $t &gt; k_i$, the $i$-th student will choose exactly $k_i$ random pinned messages (all possible subsets of pinned messages of size $k_i$ are equiprobable) and read only the chosen messages.</p><p>Monocarp wants to maximize the expected number of students that read their respective messages (i.e. the number of such indices $i$ that student $i$ reads the message $m_i$). Help him to choose how many (and which) messages should he pin!</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of students in the conference.</p><p>Then $n$ lines follow. The $i$-th line contains two integers $m_i$ and $k_i$ ($1 \le m_i \le 2 \cdot 10^5$; $1 \le k_i \le 20$) — the index of the message which Monocarp wants the $i$-th student to read and the maximum number of messages the $i$-th student will read, respectively.</p></div><div class="output-specification"><p>In the first line, print one integer $t$ ($1 \le t \le 2 \cdot 10^5$) — the number of messages Monocarp should pin. In the second line, print $t$ <span class="tex-font-style-bf">distinct</span> integers $c_1$, $c_2$, ..., $c_t$ ($1 \le c_i \le 2 \cdot 10^5$) — the indices of the messages Monocarp should pin. The messages can be listed in any order.</p><p>If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of students in the conference.</p><p>Then $n$ lines follow. The $i$-th line contains two integers $m_i$ and $k_i$ ($1 \le m_i \le 2 \cdot 10^5$; $1 \le k_i \le 20$) — the index of the message which Monocarp wants the $i$-th student to read and the maximum number of messages the $i$-th student will read, respectively.</p>

## Output

<p>In the first line, print one integer $t$ ($1 \le t \le 2 \cdot 10^5$) — the number of messages Monocarp should pin. In the second line, print $t$ <span class="tex-font-style-bf">distinct</span> integers $c_1$, $c_2$, ..., $c_t$ ($1 \le c_i \le 2 \cdot 10^5$) — the indices of the messages Monocarp should pin. The messages can be listed in any order.</p><p>If there are multiple answers, print any of them.</p>





```input1
3
10 1
10 2
5 2
```




```input2
3
10 1
5 2
10 1
```




```input3
4
1 1
2 2
3 3
4 4
```




```input4
3
13 2
42 2
37 2
```




```output1
2
5 10
```




```output2
1
10
```




```output3
3
2 3 4
```




```output4
3
42 13 37
```



## Note

<p>Let's consider the examples from the statement.</p><ol><li> In the first example, Monocarp pins the messages $5$ and $10$.<ul> <li> if the first student reads the message $5$, the second student reads the messages $5$ and $10$, and the third student reads the messages $5$ and $10$, the number of students which have read their respective messages will be $2$; </li><li> if the first student reads the message $10$, the second student reads the messages $5$ and $10$, and the third student reads the messages $5$ and $10$, the number of students which have read their respective messages will be $3$. </li></ul><p>So, the expected number of students which will read their respective messages is $\frac{5}{2}$.</p></li><li> In the second example, Monocarp pins the message $10$.<ul> <li> if the first student reads the message $10$, the second student reads the message $10$, and the third student reads the message $10$, the number of students which have read their respective messages will be $2$. </li></ul><p>So, the expected number of students which will read their respective messages is $2$. If Monocarp had pinned both messages $5$ and $10$, the expected number of students which read their respective messages would have been $2$ as well.</p></li><li> In the third example, the expected number of students which will read their respective messages is $\frac{8}{3}$.</li><li> In the fourth example, the expected number of students which will read their respective messages is $2$.</li></ol>
