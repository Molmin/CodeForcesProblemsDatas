## Description

<div><p>There are $n$ of independent carriages on the rails. The carriages are numbered from left to right from $1$ to $n$. The carriages are not connected to each other. The carriages move to the left, so that the carriage with number $1$ moves ahead of all of them.</p><p>The $i$-th carriage has its own engine, which can accelerate the carriage to $a_i$ km/h, but the carriage cannot go faster than the carriage in front of it. See example for explanation.</p><p>All carriages start moving to the left at the same time, and they naturally form <span class="tex-font-style-bf">trains</span>. We will call <span class="tex-font-style-bf">trains</span>&nbsp;— consecutive moving carriages having the same speed.</p><p>For example, we have $n=5$ carriages and array $a = [10, 13, 5, 2, 6]$. Then the final speeds of the carriages will be $[10, 10, 5, 2, 2]$. Respectively, $3$ of the train will be formed.</p><p>There are also messages saying that some engine has been corrupted:</p><ul> <li> message "<span class="tex-font-style-tt">k d</span>" means that the speed of the $k$-th carriage has decreased by $d$ (that is, there has been a change in the maximum speed of the carriage $a_k = a_k - d$). </li></ul> <p>Messages arrive sequentially, the processing of the next message takes into account the changes from all previous messages.</p><p>After each message determine the number of formed trains.</p></div><div class="input-specification"><p>The first line of input data contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;—the number of input test cases.</p><p>This is followed by descriptions of the test cases.</p><p>The first line of each test case is empty.</p><p>The second line of the test case contains two integers $n$ and $m$ ($1 \le n,m \le 10^5$)&nbsp;—the number of carriages and the number of messages to slow down the carriage, respectively.</p><p>The third line contains $n$ integers: $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 10^9$)&nbsp;— the number $a_i$ means that the carriage with number $i$ can reach a speed of $a_i$ km/h. </p><p>The next $m$ lines contain two integers $k_j$ and $d_j$ ($1 \le k_j \le n$, $0 \le d_j \le a_{k_j}$)&nbsp;—this is the message that the speed of the carriage with number $k_j$ has decreased by $d_j$. In other words, there has been a change in its maximum speed $a_{k_j} = a_{k_j} - d_j$. Note that at any time the speed of each carriage is non-negative. In other words, $a_i \ge s_i$, where $s_i$&nbsp;—is the sum of such $d_j$ that $k_j=i$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$. Similarly, it is guaranteed that the sum of $m$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>Print $t$ lines. On each line print the answer for the corresponding test case.</p><p>For each test case print $m$ numbers: the number of trains formed after each message.</p></div>

## Input

<p>The first line of input data contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;—the number of input test cases.</p><p>This is followed by descriptions of the test cases.</p><p>The first line of each test case is empty.</p><p>The second line of the test case contains two integers $n$ and $m$ ($1 \le n,m \le 10^5$)&nbsp;—the number of carriages and the number of messages to slow down the carriage, respectively.</p><p>The third line contains $n$ integers: $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 10^9$)&nbsp;— the number $a_i$ means that the carriage with number $i$ can reach a speed of $a_i$ km/h. </p><p>The next $m$ lines contain two integers $k_j$ and $d_j$ ($1 \le k_j \le n$, $0 \le d_j \le a_{k_j}$)&nbsp;—this is the message that the speed of the carriage with number $k_j$ has decreased by $d_j$. In other words, there has been a change in its maximum speed $a_{k_j} = a_{k_j} - d_j$. Note that at any time the speed of each carriage is non-negative. In other words, $a_i \ge s_i$, where $s_i$&nbsp;—is the sum of such $d_j$ that $k_j=i$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$. Similarly, it is guaranteed that the sum of $m$ over all test cases does not exceed $10^5$.</p>

## Output

<p>Print $t$ lines. On each line print the answer for the corresponding test case.</p><p>For each test case print $m$ numbers: the number of trains formed after each message.</p>





```input1
3

4 2
6 2 3 7
3 2
4 7

5 4
10 13 5 2 6
2 4
5 2
1 5
3 2

13 4
769 514 336 173 181 373 519 338 985 709 729 702 168
12 581
6 222
7 233
5 117
```




```output1
3 4 
4 4 2 3 
5 6 6 5
```



## Note

<p>For the first test case:</p><ul> <li> Initially array $a = [6, 2, 3, 7]$. </li><li> After the first message, the array $a = [6, 2, 1, 7]$. Accordingly, the speeds of the carriages are $[6, 2, 1, 1]$ and will form $3$ of the train. </li><li> After the second message the array $a = [6, 2, 1, 0]$. Accordingly, the speeds of the carriages are $[6, 2, 1, 0]$, and $4$ of the train will be formed. </li></ul><p>For the second test case:</p><ul> <li> Initially, the array $a = [10, 13, 5, 2, 6]$. </li><li> After the first message, the array $a = [10, 9, 5, 2, 6]$. Accordingly, the speeds of the carriages are equal: $[10, 9, 5, 2, 2]$, and $4$ of the train will be formed. </li><li> After the second message the array $a = [10, 9, 5, 2, 4]$. Accordingly, the speeds of the carriages are $[10, 9, 5, 2, 2]$, and $4$ of the train will be formed. </li><li> After the third message the array $a = [5, 9, 5, 2, 4]$. Accordingly, the speeds of the carriages are $[5, 5, 5, 2, 2]$, and $2$ of the train will be formed. </li><li> After the fourth message the array $a = [5, 9, 3, 2, 4]$. Accordingly, the speeds of the carriages are $[5, 5, 3, 2, 2]$, and $3$ of the train will be formed. </li></ul>
