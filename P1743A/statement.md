## Description

<div><p>Monocarp has forgotten the password to his mobile phone. The password consists of $4$ digits from $0$ to $9$ (note that it can start with the digit $0$).</p><p>Monocarp remembers that his password had exactly two different digits, and each of these digits appeared exactly two times in the password. Monocarp also remembers some digits which were definitely not used in the password.</p><p>You have to calculate the number of different sequences of $4$ digits that could be the password for Monocarp's mobile phone (i. e. these sequences should meet all constraints on Monocarp's password).</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 200$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains a single integer $n$ ($1 \le n \le 8$)&nbsp;— the number of digits for which Monocarp remembers that they were not used in the password.</p><p>The second line contains $n$ different integers $a_1, a_2, \dots a_n$ ($0 \le a_i \le 9$) representing the digits that were not used in the password. Note that the digits $a_1, a_2, \dots, a_n$ are given in ascending order.</p></div><div class="output-specification"><p>For each testcase, print one integer&nbsp;— the number of different $4$-digit sequences that meet the constraints.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 200$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains a single integer $n$ ($1 \le n \le 8$)&nbsp;— the number of digits for which Monocarp remembers that they were not used in the password.</p><p>The second line contains $n$ different integers $a_1, a_2, \dots a_n$ ($0 \le a_i \le 9$) representing the digits that were not used in the password. Note that the digits $a_1, a_2, \dots, a_n$ are given in ascending order.</p>

## Output

<p>For each testcase, print one integer&nbsp;— the number of different $4$-digit sequences that meet the constraints.</p>





```input1|2,3
2
8
0 1 2 4 5 6 8 9
1
8
```




```output1
6
216
```



## Note

<p>In the first example, all possible passwords are: "<span class="tex-font-style-tt">3377</span>", "<span class="tex-font-style-tt">3737</span>", "<span class="tex-font-style-tt">3773</span>", "<span class="tex-font-style-tt">7337</span>", "<span class="tex-font-style-tt">7373</span>", "<span class="tex-font-style-tt">7733</span>".</p>
