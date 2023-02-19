## Description

<div><p>The <span class="tex-font-style-it">score</span> of an array $v_1,v_2,\ldots,v_n$ is defined as the number of indices $i$ ($1 \le i \le n$) such that $v_1+v_2+\ldots+v_i = 0$.</p><p>You are given an array $a_1,a_2,\ldots,a_n$ of length $n$. You can perform the following operation multiple times:</p><ul> <li> select an index $i$ ($1 \le i \le n$) such that $a_i=0$; </li><li> then replace $a_i$ by an arbitrary integer. </li></ul> <p>What is the maximum possible score of $a$ that can be obtained by performing a sequence of such operations?</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the length of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1,a_2,\ldots,a_n$ ($-10^9 \le a_i \le 10^9$)&nbsp;— array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print the maximum possible score of the array $a$ after performing a sequence of operations.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the length of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1,a_2,\ldots,a_n$ ($-10^9 \le a_i \le 10^9$)&nbsp;— array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print the maximum possible score of the array $a$ after performing a sequence of operations.</p>





```input1|2,3,6,7,10,11
5
5
2 0 1 -1 0
3
1000000000 1000000000 0
4
0 0 0 0
8
3 0 2 -10 10 -30 30 0
9
1 0 0 1 -1 0 1 0 -1
```




```output1
3
1
4
4
5
```



## Note

<p>In the first test case, it is optimal to change the value of $a_2$ to $-2$ in one operation.</p><p>The resulting array $a$ will be $[2,-2,1,-1,0]$, with a score of $3$:</p><ul> <li> $a_1+a_2=2-2=0$; </li><li> $a_1+a_2+a_3+a_4=2-2+1-1=0$; </li><li> $a_1+a_2+a_3+a_4+a_5=2-2+1-1+0=0$. </li></ul><p>In the second test case, it is optimal to change the value of $a_3$ to $-2\,000\,000\,000$, giving us an array with a score of $1$.</p><p>In the third test case, it is not necessary to perform any operations.</p>
