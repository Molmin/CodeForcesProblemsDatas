## Description

<div><p>Define a cyclic sequence of size $n$ as an array $s$ of length $n$, in which $s_n$ is adjacent to $s_1$.</p><p>Muxii has a ring represented by a cyclic sequence $a$ of size $n$.</p><p>However, the ring itself hates equal adjacent elements. So if two adjacent elements in the sequence are equal at any time, <span class="tex-font-style-bf">one of them</span> will be erased <span class="tex-font-style-bf">immediately</span>. The sequence doesn't contain equal adjacent elements initially.</p><p>Muxii can perform the following operation until the sequence becomes empty:</p><ul> <li> Choose an element in $a$ and erase it. </li></ul><p>For example, if ring is $[1, 2, 4, 2, 3, 2]$, and Muxii erases element $4$, then ring would erase one of the elements equal to $2$, and the ring will become $[1, 2, 3, 2]$.</p><p>Muxii wants to find the <span class="tex-font-style-bf">maximum</span> number of operations he could perform.</p><p><span class="tex-font-style-bf">Note that in a ring of size $1$, its only element isn't considered adjacent to itself (so it's not immediately erased).</span></p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1\leq t\leq 100$)&nbsp;— the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1\leq n\leq 100$)&nbsp;— the size of the cyclic sequence.</p><p>The second line of each test case contains $n$ integers $a_1,a_2,\ldots,a_n$ ($1\leq a_i\leq n$)&nbsp;— the sequence itself.</p><p>It's guaranteed that $a_i\ne a_{i+1}$ for $1\leq i&lt;n$.</p><p>It's guaranteed that $a_n\ne a_1$ when $n&gt;1$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;— the maximum number of operations Muxii can perform.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1\leq t\leq 100$)&nbsp;— the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1\leq n\leq 100$)&nbsp;— the size of the cyclic sequence.</p><p>The second line of each test case contains $n$ integers $a_1,a_2,\ldots,a_n$ ($1\leq a_i\leq n$)&nbsp;— the sequence itself.</p><p>It's guaranteed that $a_i\ne a_{i+1}$ for $1\leq i&lt;n$.</p><p>It's guaranteed that $a_n\ne a_1$ when $n&gt;1$.</p>

## Output

<p>For each test case, output a single integer&nbsp;— the maximum number of operations Muxii can perform.</p>





```input1|2,3,6,7
3
4
1 2 3 2
4
1 2 1 2
1
1
```




```output1
4
3
1
```



## Note

<p>In the first test case, you can erase the second element first, then erase the remaining elements one by one in any order. In total, you can perform the operation $4$ times. Note that if you erase the first element first, then the sequence will be turned into $[2,3,2]$ and then immediately become $[2,3]$.</p><p>In the second test case, you can erase the first element first, then the sequence becomes $[2,1]$. Then you can erase all remaining elements one by one in any order.</p>
