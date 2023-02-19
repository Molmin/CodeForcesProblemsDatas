## Description

<div><p>You are given an array $a$ of $n$ integers. Initially there is only one copy of the given array.</p><p>You can do operations of two types:</p><ol> <li> Choose any array and clone it. After that there is one more copy of the chosen array. </li><li> Swap two elements from <span class="tex-font-style-bf">any</span> two copies (maybe in the same copy) on any positions. </li></ol><p>You need to find the minimal number of operations needed to obtain a copy where all elements are equal.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;— the length of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-10^9 \le a_i \le 10^9$)&nbsp;— the elements of the array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case output a single integer&nbsp;— the minimal number of operations needed to create at least one copy where all elements are equal.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;— the length of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-10^9 \le a_i \le 10^9$)&nbsp;— the elements of the array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case output a single integer&nbsp;— the minimal number of operations needed to create at least one copy where all elements are equal.</p>





```input1
6
1
1789
6
0 1 3 3 7 0
2
-1000000000 1000000000
4
4 3 2 1
5
2 5 7 6 3
7
1 1 1 1 1 1 1
```




```output1
0
6
2
5
7
0
```



## Note

<p>In the first test case all elements in the array are already equal, that's why the answer is $0$.</p><p>In the second test case it is possible to create a copy of the given array. After that there will be two identical arrays:</p><p>$[ \ 0 \ 1 \ 3 \ 3 \ 7 \ 0 \ ]$ and $[ \ 0 \ 1 \ 3 \ 3 \ 7 \ 0 \ ]$</p><p>After that we can swap elements in a way so all zeroes are in one array:</p><p>$[ \ 0 \ \underline{0} \ \underline{0} \ 3 \ 7 \ 0 \ ]$ and $[ \ \underline{1} \ 1 \ 3 \ 3 \ 7 \ \underline{3} \ ]$</p><p>Now let's create a copy of the first array:</p><p>$[ \ 0 \ 0 \ 0 \ 3 \ 7 \ 0 \ ]$, $[ \ 0 \ 0 \ 0 \ 3 \ 7 \ 0 \ ]$ and $[ \ 1 \ 1 \ 3 \ 3 \ 7 \ 3 \ ]$</p><p>Let's swap elements in the first two copies:</p><p>$[ \ 0 \ 0 \ 0 \ \underline{0} \ \underline{0} \ 0 \ ]$, $[ \ \underline{3} \ \underline{7} \ 0 \ 3 \ 7 \ 0 \ ]$ and $[ \ 1 \ 1 \ 3 \ 3 \ 7 \ 3 \ ]$.</p><p>Finally, we made a copy where all elements are equal and made $6$ operations.</p><p>It can be proven that no fewer operations are enough.</p>
