## Description

<div><p>Students of one unknown college don't have PE courses. That's why $q$ of them decided to visit a gym nearby by themselves. The gym is open for $n$ days and has a ticket system. At the $i$-th day, the cost of one ticket is equal to $a_i$. You are free to buy more than one ticket per day.</p><p>You can activate a ticket purchased at day $i$ either at day $i$ or any day later. Each activated ticket is valid only for $k$ days. In other words, if you activate ticket at day $t$, it will be valid only at days $t, t + 1, \dots, t + k - 1$. </p><p>You know that the $j$-th student wants to visit the gym at each day from $l_j$ to $r_j$ inclusive. Each student will use the following strategy of visiting the gym at any day $i$ ($l_j \le i \le r_j$):</p><ol> <li> person comes to a desk selling tickets placed near the entrance and buy several tickets with cost $a_i$ apiece (possibly, zero tickets); </li><li> if the person has at least one activated and still valid ticket, they just go in. Otherwise, they activate one of tickets purchased today or earlier and go in. </li></ol><p>Note that each student will visit gym only starting $l_j$, so each student has to buy at least one ticket at day $l_j$.</p><p>Help students to calculate the minimum amount of money they have to spend in order to go to the gym.</p></div><div class="input-specification"><p>The first line contains three integers $n$, $q$ and $k$ ($1 \le n, q \le 300\,000$; $1 \le k \le n$)&nbsp;— the number of days, the number of students and the number of days each ticket is still valid. </p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the cost of one ticket at the corresponding day.</p><p>Each of the next $q$ lines contains two integers $l_i$ and $r_i$ ($1 \le l_i \le r_i \le n$)&nbsp;— the segment of days the corresponding student want to visit the gym.</p></div><div class="output-specification"><p>For each student, print the minimum possible amount of money they have to spend in order to go to the gym at desired days.</p></div>

## Input

<p>The first line contains three integers $n$, $q$ and $k$ ($1 \le n, q \le 300\,000$; $1 \le k \le n$)&nbsp;— the number of days, the number of students and the number of days each ticket is still valid. </p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the cost of one ticket at the corresponding day.</p><p>Each of the next $q$ lines contains two integers $l_i$ and $r_i$ ($1 \le l_i \le r_i \le n$)&nbsp;— the segment of days the corresponding student want to visit the gym.</p>

## Output

<p>For each student, print the minimum possible amount of money they have to spend in order to go to the gym at desired days.</p>





```input1
7 5 2
2 15 6 3 7 5 6
1 2
3 7
5 5
7 7
3 5
```




```output1
2
12
7
6
9
```



## Note

<p>Let's see how each student have to spend their money: </p><ul> <li> The first student should buy one ticket at day $1$. </li><li> The second student should buy one ticket at day $3$ and two tickets at day $4$. Note that student can keep purchased tickets for the next days. </li><li> The third student should buy one ticket at day $5$. </li><li> The fourth student should buy one ticket at day $7$. </li><li> The fifth student should buy one ticket at day $3$ and one at day $4$. </li></ul>
