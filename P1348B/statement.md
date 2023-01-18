## Description

<div><p>Phoenix loves beautiful arrays. An array is beautiful if all its subarrays of length&nbsp;$k$ have the same sum. A subarray of an array is any sequence of consecutive elements.</p><p>Phoenix currently has an array $a$ of length $n$. He wants to insert some number of integers, possibly zero, into his array such that it becomes beautiful. The inserted integers must be between $1$ and $n$ inclusive. Integers may be inserted anywhere (even before the first or after the last element), and he is <span class="tex-font-style-bf">not trying</span> to minimize the number of inserted integers.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \le t \le 50$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le k \le n \le 100$).</p><p>The second line of each test case contains $n$ space-separated integers ($1 \le a_i \le n$)&nbsp;— the array that Phoenix currently has. This array may or may not be already beautiful.</p></div><div class="output-specification"><p>For each test case, if it is impossible to create a beautiful array, print <span class="tex-font-style-tt">-1</span>. Otherwise, print two lines.</p><p>The first line should contain the length of the beautiful array $m$ ($n \le m \le 10^4$). You don't need to minimize $m$.</p><p>The second line should contain $m$ space-separated integers ($1 \le b_i \le n$)&nbsp;— a beautiful array that Phoenix can obtain after inserting some, possibly zero, integers into his array $a$. You may print integers that weren't originally in array $a$.</p><p>If there are multiple solutions, print any. It's guaranteed that if we can make array $a$ beautiful, we can always make it with resulting length no more than $10^4$.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \le t \le 50$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le k \le n \le 100$).</p><p>The second line of each test case contains $n$ space-separated integers ($1 \le a_i \le n$)&nbsp;— the array that Phoenix currently has. This array may or may not be already beautiful.</p>

## Output

<p>For each test case, if it is impossible to create a beautiful array, print <span class="tex-font-style-tt">-1</span>. Otherwise, print two lines.</p><p>The first line should contain the length of the beautiful array $m$ ($n \le m \le 10^4$). You don't need to minimize $m$.</p><p>The second line should contain $m$ space-separated integers ($1 \le b_i \le n$)&nbsp;— a beautiful array that Phoenix can obtain after inserting some, possibly zero, integers into his array $a$. You may print integers that weren't originally in array $a$.</p><p>If there are multiple solutions, print any. It's guaranteed that if we can make array $a$ beautiful, we can always make it with resulting length no more than $10^4$.</p>





```input1
4
4 2
1 2 2 1
4 3
1 2 2 1
3 2
1 2 3
4 4
4 3 4 2
```




```output1
5
1 2 1 2 1
4
1 2 2 1
-1
7
4 3 2 1 4 3 2
```



## Note

<p>In the first test case, we can make array $a$ beautiful by inserting the integer $1$ at index $3$ (in between the two existing $2$s). Now, all subarrays of length $k=2$ have the same sum $3$. There exists many other possible solutions, for example: </p><ul> <li> $2, 1, 2, 1, 2, 1$ </li><li> $1, 2, 1, 2, 1, 2$ </li></ul><p>In the second test case, the array is already beautiful: all subarrays of length $k=3$ have the same sum $5$.</p><p>In the third test case, it can be shown that we cannot insert numbers to make array $a$ beautiful.</p><p>In the fourth test case, the array $b$ shown is beautiful and all subarrays of length $k=4$ have the same sum $10$. There exist other solutions also.</p>
