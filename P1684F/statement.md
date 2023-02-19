## Description

<div><p>You are given an array $a$ of $n$ integers. Also you are given $m$ subsegments of that array. The left and the right endpoints of the $j$-th segment are $l_j$ and $r_j$ respectively.</p><p>You are allowed to make <span class="tex-font-style-bf">no more than one</span> operation. In that operation you choose any subsegment of the array $a$ and replace each value on this segment with any integer (you are also allowed to keep elements the same).</p><p>You have to apply this operation so that for the given $m$ segments, the elements on each segment are distinct. More formally, for each $1 \le j \le m$ all elements $a_{l_{j}}, a_{l_{j}+1}, \ldots, a_{r_{j}-1}, a_{r_{j}}$ should be distinct.</p><p>You don't want to use the operation on a big segment, so you have to find the smallest length of a segment, so that you can apply the operation to this segment and meet the above-mentioned conditions. If it is not needed to use this operation, the answer is $0$.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n, m \le 2 \cdot 10^5$)&nbsp;— the size of the array and the number of segments respectively.</p><p>The next line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the elements of $a$.</p><p>Each of the next $m$ lines contains two integers $l_j$, $r_j$ ($1 \le l_j \le r_j \le n$)&nbsp;— the left and the right endpoints of the $j$-th segment.</p><p>It's guaranteed that the sum of $n$ and the sum of $m$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case output a single integer&nbsp;— the smallest length of a segment you can apply an operation on making the elements on all given segments distinct. If it is not needed to use the operation, output $0$.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n, m \le 2 \cdot 10^5$)&nbsp;— the size of the array and the number of segments respectively.</p><p>The next line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the elements of $a$.</p><p>Each of the next $m$ lines contains two integers $l_j$, $r_j$ ($1 \le l_j \le r_j \le n$)&nbsp;— the left and the right endpoints of the $j$-th segment.</p><p>It's guaranteed that the sum of $n$ and the sum of $m$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case output a single integer&nbsp;— the smallest length of a segment you can apply an operation on making the elements on all given segments distinct. If it is not needed to use the operation, output $0$.</p>





```input1|2,3,4,5,6,11,12,13,14,15,16,17,23,24,25
5
7 3
1 1 2 1 3 3 5
1 4
4 5
2 4
5 2
10 1 6 14 1
4 5
2 4
4 5
5 7 5 6
2 2
1 3
2 4
3 3
3 4
7 3
2 2 2 7 8 2 2
4 4
4 4
5 5
1 1
123
1 1
```




```output1
2
0
1
0
0
```



## Note

<p>In the first test case you can perform the operation on the segment $[1, 2]$ and make $a = [5, 6, 2, 1, 3, 3, 5]$. Then the elements on each segment are distinct.</p><ul> <li> On the segment $[1, 4]$ there are $[5, 6, 2, 1]$. </li><li> On the segment $[4, 5]$ there are $[1, 3]$. </li><li> On the segment $[2, 4]$ there are $[6, 2, 1, 3]$. </li></ul><p>This way on each of the given segments all elements are distinct. Also, it is impossible to change any single integer to make elements distinct on each segment. That is why the answer is $2$.</p><p>In the second test case the elements on each segment are already distinct, so we should not perform the operation.</p><p>In the third test case we can replace the first $5$ by $1$. This way we will get $[1, 7, 5, 6]$ where all elements are distinct so on each given segment all elements are distinct.</p>
