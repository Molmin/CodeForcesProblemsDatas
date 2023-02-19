## Description

<div><p><span class="tex-font-style-it">This is the hard version of the problem. The only difference between the two versions is that the harder version asks additionally for a minimum number of subsegments.</span></p><p>Tokitsukaze has a binary string $s$ of length $n$, consisting only of zeros and ones, $n$ is <span class="tex-font-style-bf">even</span>.</p><p>Now Tokitsukaze divides $s$ into <span class="tex-font-style-bf">the minimum number</span> of <span class="tex-font-style-bf">contiguous</span> subsegments, and for each subsegment, all bits in each subsegment are the same. After that, $s$ is considered good if the lengths of all subsegments are even.</p><p>For example, if $s$ is "<span class="tex-font-style-tt">11001111</span>", it will be divided into "<span class="tex-font-style-tt">11</span>", "<span class="tex-font-style-tt">00</span>" and "<span class="tex-font-style-tt">1111</span>". Their lengths are $2$, $2$, $4$ respectively, which are all even numbers, so "<span class="tex-font-style-tt">11001111</span>" is good. Another example, if $s$ is "<span class="tex-font-style-tt">1110011000</span>", it will be divided into "<span class="tex-font-style-tt">111</span>", "<span class="tex-font-style-tt">00</span>", "<span class="tex-font-style-tt">11</span>" and "<span class="tex-font-style-tt">000</span>", and their lengths are $3$, $2$, $2$, $3$. Obviously, "<span class="tex-font-style-tt">1110011000</span>" is not good.</p><p>Tokitsukaze wants to make $s$ good by changing the values of some positions in $s$. Specifically, she can perform the operation any number of times: change the value of $s_i$ to '<span class="tex-font-style-tt">0</span>' or '<span class="tex-font-style-tt">1</span>' ($1 \leq i \leq n$). Can you tell her the minimum number of operations to make $s$ good? <span class="tex-font-style-bf">Meanwhile, she also wants to know the minimum number of subsegments that $s$ can be divided into among all solutions with the minimum number of operations.</span></p></div><div class="input-specification"><p>The first contains a single positive integer $t$ ($1 \leq t \leq 10\,000$)&nbsp;— the number of test cases.</p><p>For each test case, the first line contains a single integer $n$ ($2 \leq n \leq 2 \cdot 10^5$)&nbsp;— the length of $s$, it is guaranteed that $n$ is even.</p><p>The second line contains a binary string $s$ of length $n$, consisting only of zeros and ones.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print a single line with two integers&nbsp;— the minimum number of operations to make $s$ good, and the minimum number of subsegments that $s$ can be divided into among all solutions with the minimum number of operations.</p></div>

## Input

<p>The first contains a single positive integer $t$ ($1 \leq t \leq 10\,000$)&nbsp;— the number of test cases.</p><p>For each test case, the first line contains a single integer $n$ ($2 \leq n \leq 2 \cdot 10^5$)&nbsp;— the length of $s$, it is guaranteed that $n$ is even.</p><p>The second line contains a binary string $s$ of length $n$, consisting only of zeros and ones.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print a single line with two integers&nbsp;— the minimum number of operations to make $s$ good, and the minimum number of subsegments that $s$ can be divided into among all solutions with the minimum number of operations.</p>





```input1|2,3,6,7,10,11
5
10
1110011000
8
11001111
2
00
2
11
6
100110
```




```output1
3 2
0 3
0 1
0 1
3 1
```



## Note

<p>In the first test case, one of the ways to make $s$ good is the following.</p><p>Change $s_3$, $s_6$ and $s_7$ to '<span class="tex-font-style-tt">0</span>', after that $s$ becomes "<span class="tex-font-style-tt">1100000000</span>", it can be divided into "<span class="tex-font-style-tt">11</span>" and "<span class="tex-font-style-tt">00000000</span>", which lengths are $2$ and $8$ respectively, the number of subsegments of it is $2$. There are other ways to operate $3$ times to make $s$ good, such as "<span class="tex-font-style-tt">1111110000</span>", "<span class="tex-font-style-tt">1100001100</span>", "<span class="tex-font-style-tt">1111001100</span>", the number of subsegments of them are $2$, $4$, $4$ respectively. It's easy to find that the minimum number of subsegments among all solutions with the minimum number of operations is $2$.</p><p>In the second, third and fourth test cases, $s$ is good initially, so no operation is required.</p>
