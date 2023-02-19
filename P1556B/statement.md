## Description

<div><center> <img class="tex-graphics" height="302px" src="file://3X30V6YA.png" style="max-width: 100.0%;max-height: 100.0%;" width="454px"> </center><p>William has an array of $n$ integers $a_1, a_2, \dots, a_n$. In one move he can swap two neighboring items. Two items $a_i$ and $a_j$ are considered neighboring if the condition $|i - j| = 1$ is satisfied.</p><p>William wants you to calculate the minimal number of swaps he would need to perform to make it so that the array does not contain two neighboring items with the same parity.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). Description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ $(1 \le n \le 10^5)$ which is the total number of items in William's array.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ $(1 \le a_i \le 10^9)$ which are William's array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case output the minimal number of operations needed or $-1$ if it is impossible to get the array to a state when no neighboring numbers have the same parity.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). Description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ $(1 \le n \le 10^5)$ which is the total number of items in William's array.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ $(1 \le a_i \le 10^9)$ which are William's array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case output the minimal number of operations needed or $-1$ if it is impossible to get the array to a state when no neighboring numbers have the same parity.</p>





```input1
5
3
6 6 1
1
9
6
1 1 1 2 2 2
2
8 6
6
6 2 3 4 5 1
```




```output1
1
0
3
-1
2
```



## Note

<p>In the first test case the following sequence of operations would satisfy the requirements: </p><ol> <li> swap(2, 3). Array after performing the operation: $[6, 1, 6]$ </li></ol><p>In the second test case the array initially does not contain two neighboring items of the same parity.</p><p>In the third test case the following sequence of operations would satisfy the requirements: </p><ol> <li> swap(3, 4). Array after performing the operation: $[1, 1, 2, 1, 2, 2]$ </li><li> swap(2, 3). Array after performing the operation: $[1, 2, 1, 1, 2, 2]$ </li><li> swap(4, 5). Array after performing the operation: $[1, 2, 1, 2, 1, 2]$ </li></ol><p>In the fourth test case it is impossible to satisfy the requirements.</p><p>In the fifth test case the following sequence of operations would satisfy the requirements: </p><ol> <li> swap(2, 3). Array after performing the operation: $[6, 3, 2, 4, 5, 1]$ </li><li> swap(4, 5). Array after performing the operation: $[6, 3, 2, 5, 4, 1]$ </li></ol>
