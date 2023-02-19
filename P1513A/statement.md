## Description

<div><p>A sequence of $n$ integers is called a permutation if it contains all integers from $1$ to $n$ exactly once.</p><p>Given two integers $n$ and $k$, construct a permutation $a$ of numbers from $1$ to $n$ which has <span class="tex-font-style-bf">exactly</span> $k$ peaks. An index $i$ of an array $a$ of size $n$ is said to be a peak if $1 &lt; i &lt; n$ and $a_i \gt a_{i-1}$ and $a_i \gt a_{i+1}$. If such permutation is not possible, then print $-1$.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases.</p><p>Then $t$ lines follow, each containing two space-separated integers $n$ ($1 \leq n \leq 100$) and $k$ ($0 \leq k \leq n$)&nbsp;— the length of an array and the required number of peaks.</p></div><div class="output-specification"><p>Output $t$ lines. For each test case, if there is no permutation with given length and number of peaks, then print $-1$. Otherwise print a line containing $n$ space-separated integers which forms a permutation of numbers from $1$ to $n$ and contains exactly $k$ peaks. </p><p>If there are multiple answers, print any.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases.</p><p>Then $t$ lines follow, each containing two space-separated integers $n$ ($1 \leq n \leq 100$) and $k$ ($0 \leq k \leq n$)&nbsp;— the length of an array and the required number of peaks.</p>

## Output

<p>Output $t$ lines. For each test case, if there is no permutation with given length and number of peaks, then print $-1$. Otherwise print a line containing $n$ space-separated integers which forms a permutation of numbers from $1$ to $n$ and contains exactly $k$ peaks. </p><p>If there are multiple answers, print any.</p>





```input1
5
1 0
5 2
6 6
2 1
6 1
```




```output1
1 
2 4 1 5 3 
-1
-1
1 3 6 5 4 2
```



## Note

<p>In the second test case of the example, we have array $a = [2,4,1,5,3]$. Here, indices $i=2$ and $i=4$ are the peaks of the array. This is because $(a_{2} \gt a_{1} $, $a_{2} \gt a_{3})$ and $(a_{4} \gt a_{3}$, $a_{4} \gt a_{5})$. </p>
