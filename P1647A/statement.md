## Description

<div><p>Madoka finally found the administrator password for her computer. Her father is a well-known popularizer of mathematics, so the password is the answer to the following problem.</p><p>Find the maximum decimal number without zeroes and with no equal digits in a row, such that the sum of its digits is $n$.</p><p>Madoka is too tired of math to solve it herself, so help her to solve this problem!</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The only line of each test case contains an integer $n$ ($1 \le n \le 1000$)&nbsp;— the required sum of the digits.</p></div><div class="output-specification"><p>For each test case print the maximum number you can obtain.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The only line of each test case contains an integer $n$ ($1 \le n \le 1000$)&nbsp;— the required sum of the digits.</p>

## Output

<p>For each test case print the maximum number you can obtain.</p>





```input1
5
1
2
3
4
5
```




```output1
1
2
21
121
212
```



## Note

<p>The only numbers with the sum of digits equal to $2$ without zeros are $2$ and $11$. But the last one has two ones in a row, so it's not valid. That's why the answer is $2$.</p><p>The only numbers with the sum of digits equal to $3$ without zeros are $111$, $12$, $21$, and $3$. The first one has $2$ ones in a row, so it's not valid. So the maximum valid number is $21$.</p><p>The only numbers with the sum of digits equals to $4$ without zeros are $1111$, $211$, $121$, $112$, $13$, $31$, $22$, and $4$. Numbers $1111$, $211$, $112$, $22$ aren't valid, because they have some identical digits in a row. So the maximum valid number is $121$.</p>
