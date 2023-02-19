## Description

<div><p>Polycarp got an array of integers $a[1 \dots n]$ as a gift. Now he wants to perform a certain number of operations (possibly zero) so that all elements of the array become the same (that is, to become $a_1=a_2=\dots=a_n$).</p><ul><li> In one operation, he can take some indices in the array and increase the elements of the array at those indices by $1$.</li></ul><p>For example, let $a=[4,2,1,6,2]$. He can perform the following operation: select indices 1, 2, and 4 and increase elements of the array in those indices by $1$. As a result, in one operation, he can get a new state of the array $a=[5,3,1,7,2]$.</p><p>What is the minimum number of operations it can take so that all elements of the array become equal to each other (that is, to become $a_1=a_2=\dots=a_n$)?</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ ($1 \le t \le 10^4$) &nbsp;— the number of test cases in the test.</p><p>The following are descriptions of the input test cases.</p><p>The first line of the description of each test case contains one integer $n$ ($1 \le n \le 50$) &nbsp;— the array $a$.</p><p>The second line of the description of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$) &nbsp;— elements of the array $a$.</p></div><div class="output-specification"><p>For each test case, print one integer &nbsp;— the minimum number of operations to make all elements of the array $a$ equal.</p></div>

## Input

<p>The first line of the input contains a single integer $t$ ($1 \le t \le 10^4$) &nbsp;— the number of test cases in the test.</p><p>The following are descriptions of the input test cases.</p><p>The first line of the description of each test case contains one integer $n$ ($1 \le n \le 50$) &nbsp;— the array $a$.</p><p>The second line of the description of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$) &nbsp;— elements of the array $a$.</p>

## Output

<p>For each test case, print one integer &nbsp;— the minimum number of operations to make all elements of the array $a$ equal.</p>





```input1
3
6
3 4 2 4 1 2
3
1000 1002 998
2
12 11
```




```output1
3
4
1
```



## Note

<p>First test case: </p><ul> <li> $a=[3,4,2,4,1,2]$ take $a_3, a_5$ and perform an operation plus one on them, as a result we get $a=[3,4,3,4,2,2]$. </li><li> $a=[3,4,3,4,2,2]$ we take $a_1, a_5, a_6$ and perform an operation on them plus one, as a result we get $a=[4,4,3,4,3,3]$. </li><li> $a=[4,4,3,4,3,3]$ we take $a_3, a_5, a_6$ and perform an operation on them plus one, as a result we get $a=[4,4,4,4,4,4]$. </li></ul><p>There are other sequences of $3$ operations, after the application of which all elements become equal.</p><p>Second test case: </p><ul> <li> $a=[1000,1002,998]$ 2 times we take $a_1, a_3$ and perform an operation plus one on them, as a result we get $a=[1002,1002,1000]$. </li><li> $a=[1002,1002,1000]$ also take $a_3$ 2 times and perform an operation plus one on it, as a result we get $a=[1002,1002,1002]$. </li></ul><p>Third test case: </p><ul> <li> $a=[12,11]$ take $a_2$ and perform an operation plus one on it, as a result we get $a=[12,12]$. </li></ul>
