## Description

<div><p>Recently in Divanovo, a huge river locks system was built. There are now $n$ locks, the $i$-th of them has the volume of $v_i$ liters, so that it can contain any amount of water between $0$ and $v_i$ liters. Each lock has a pipe attached to it. When the pipe is open, $1$ liter of water enters the lock every second.</p><p>The locks system is built in a way to immediately transfer all water exceeding the volume of the lock $i$ to the lock $i + 1$. If the lock $i + 1$ is also full, water will be transferred further. Water exceeding the volume of the last lock pours out to the river. </p><center> <img class="tex-graphics" src="file://jfEMNsVb.png" style="max-width: 100.0%;max-height: 100.0%;" width="567px"> <span class="tex-font-size-small">The picture illustrates $5$ locks with two open pipes at locks $1$ and $3$. Because locks $1$, $3$, and $4$ are already filled, effectively the water goes to locks $2$ and $5$.</span> </center><p>Note that the volume of the $i$-th lock may be greater than the volume of the $i + 1$-th lock.</p><p>To make all locks work, you need to completely fill each one of them. The mayor of Divanovo is interested in $q$ independent queries. For each query, suppose that initially all locks are empty and all pipes are closed. Then, some pipes are opened simultaneously. For the $j$-th query the mayor asks you to calculate the minimum number of pipes to open so that all locks are filled no later than after $t_j$ seconds.</p><p>Please help the mayor to solve this tricky problem and answer his queries. </p></div><div class="input-specification"><p>The first lines contains one integer $n$ ($1 \le n \le 200\,000$)&nbsp;— the number of locks. </p><p>The second lines contains $n$ integers $v_1, v_2, \dots, v_n$ ($1 \le v_i \le 10^9$))&nbsp;— volumes of the locks. </p><p>The third line contains one integer $q$ ($1 \le q \le 200\,000$)&nbsp;— the number of queries. </p><p>Each of the next $q$ lines contains one integer $t_j$ ($1 \le t_j \le 10^9$)&nbsp;— the number of seconds you have to fill all the locks in the query $j$. </p></div><div class="output-specification"><p>Print $q$ integers. The $j$-th of them should be equal to the minimum number of pipes to turn on so that after $t_j$ seconds all of the locks are filled. If it is impossible to fill all of the locks in given time, print $-1$. </p></div>

## Input

<p>The first lines contains one integer $n$ ($1 \le n \le 200\,000$)&nbsp;— the number of locks. </p><p>The second lines contains $n$ integers $v_1, v_2, \dots, v_n$ ($1 \le v_i \le 10^9$))&nbsp;— volumes of the locks. </p><p>The third line contains one integer $q$ ($1 \le q \le 200\,000$)&nbsp;— the number of queries. </p><p>Each of the next $q$ lines contains one integer $t_j$ ($1 \le t_j \le 10^9$)&nbsp;— the number of seconds you have to fill all the locks in the query $j$. </p>

## Output

<p>Print $q$ integers. The $j$-th of them should be equal to the minimum number of pipes to turn on so that after $t_j$ seconds all of the locks are filled. If it is impossible to fill all of the locks in given time, print $-1$. </p>





```input1
5
4 1 5 4 1
6
1
6
2
3
4
5
```




```input2
5
4 4 4 4 4
6
1
3
6
5
2
4
```




```output1
-1
3
-1
-1
4
3
```




```output2
-1
-1
4
4
-1
5
```



## Note

<p>There are $6$ queries in the first example test. </p><p>In the queries $1, 3, 4$ the answer is $-1$. We need to wait $4$ seconds to fill the first lock even if we open all the pipes. </p><p>In the sixth query we can open pipes in locks $1$, $3$, and $4$. After $4$ seconds the locks $1$ and $4$ are full. In the following $1$ second $1$ liter of water is transferred to the locks $2$ and $5$. The lock $3$ is filled by its own pipe. </p><p>Similarly, in the second query one can open pipes in locks $1$, $3$, and $4$.</p><p>In the fifth query one can open pipes $1, 2, 3, 4$. </p>
