## Description

<div><p>You are given an array $a[0 \ldots n-1]$ of length $n$ which consists of non-negative integers. <span class="tex-font-style-bf">Note that array indices start from zero.</span></p><p>An array is called <span class="tex-font-style-it">good</span> if the parity of each index matches the parity of the element at that index. More formally, an array is good if for all $i$ ($0 \le i \le n - 1$) the equality $i \bmod 2 = a[i] \bmod 2$ holds, where $x \bmod 2$ is the remainder of dividing $x$ by 2.</p><p>For example, the arrays [$0, 5, 2, 1$] and [$0, 17, 0, 3$] are good, and the array [$2, 4, 6, 7$] is bad, because for $i=1$, the parities of $i$ and $a[i]$ are different: $i \bmod 2 = 1 \bmod 2 = 1$, but $a[i] \bmod 2 = 4 \bmod 2 = 0$.</p><p>In one move, you can take <span class="tex-font-style-bf">any</span> two elements of the array and swap them (these elements are not necessarily adjacent).</p><p>Find the minimum number of moves in which you can make the array $a$ good, or say that this is not possible.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases in the test. Then $t$ test cases follow.</p><p>Each test case starts with a line containing an integer $n$ ($1 \le n \le 40$)&nbsp;— the length of the array $a$.</p><p>The next line contains $n$ integers $a_0, a_1, \ldots, a_{n-1}$ ($0 \le a_i \le 1000$)&nbsp;— the initial array.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;— the minimum number of moves to make the given array $a$ good, or <span class="tex-font-style-tt">-1</span> if this is not possible.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases in the test. Then $t$ test cases follow.</p><p>Each test case starts with a line containing an integer $n$ ($1 \le n \le 40$)&nbsp;— the length of the array $a$.</p><p>The next line contains $n$ integers $a_0, a_1, \ldots, a_{n-1}$ ($0 \le a_i \le 1000$)&nbsp;— the initial array.</p>

## Output

<p>For each test case, output a single integer&nbsp;— the minimum number of moves to make the given array $a$ good, or <span class="tex-font-style-tt">-1</span> if this is not possible.</p>





```input1
4
4
3 2 7 6
3
3 2 6
1
7
7
4 9 2 1 18 3 0
```




```output1
2
1
-1
0
```



## Note

<p>In the first test case, in the first move, you can swap the elements with indices $0$ and $1$, and in the second move, you can swap the elements with indices $2$ and $3$.</p><p>In the second test case, in the first move, you need to swap the elements with indices $0$ and $1$.</p><p>In the third test case, you cannot make the array good.</p>
