## Description

<div><p>Spring has come, and the management of the AvtoBus bus fleet has given the order to replace winter tires with summer tires on all buses.</p><p>You own a small bus service business and you have just received an order to replace $n$ tires. You know that the bus fleet owns two types of buses: with two axles (these buses have $4$ wheels) and with three axles (these buses have $6$ wheels).</p><p>You don't know how many buses of which type the AvtoBus bus fleet owns, so you wonder how many buses the fleet might have. You have to determine the minimum and the maximum number of buses that can be in the fleet if you know that the total number of wheels for all buses is $n$.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 1\,000$)&nbsp;— the number of test cases. The following lines contain description of test cases.</p><p>The only line of each test case contains one integer $n$ ($1 \le n \le 10^{18}$)&nbsp;— the total number of wheels for all buses.</p></div><div class="output-specification"><p>For each test case print the answer in a single line using the following format.</p><p>Print two integers $x$ and $y$ ($1 \le x \le y$)&nbsp;— the minimum and the maximum possible number of buses that can be in the bus fleet.</p><p>If there is no suitable number of buses for the given $n$, print the number $-1$ as the answer.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 1\,000$)&nbsp;— the number of test cases. The following lines contain description of test cases.</p><p>The only line of each test case contains one integer $n$ ($1 \le n \le 10^{18}$)&nbsp;— the total number of wheels for all buses.</p>

## Output

<p>For each test case print the answer in a single line using the following format.</p><p>Print two integers $x$ and $y$ ($1 \le x \le y$)&nbsp;— the minimum and the maximum possible number of buses that can be in the bus fleet.</p><p>If there is no suitable number of buses for the given $n$, print the number $-1$ as the answer.</p>





```input1
4
4
7
24
998244353998244352
```




```output1
1 1
-1
4 6
166374058999707392 249561088499561088
```



## Note

<p>In the first test case the total number of wheels is $4$. It means that there is the only one bus with two axles in the bus fleet.</p><p>In the second test case it's easy to show that there is no suitable number of buses with $7$ wheels in total.</p><p>In the third test case the total number of wheels is $24$. The following options are possible:</p><ul> <li> Four buses with three axles. </li><li> Three buses with two axles and two buses with three axles. </li><li> Six buses with two axles. </li></ul><p>So the minimum number of buses is $4$ and the maximum number of buses is $6$.</p>
