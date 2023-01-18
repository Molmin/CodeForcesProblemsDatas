## Description

<div><p>You are given a long decimal number $a$ consisting of $n$ digits from $1$ to $9$. You also have a function $f$ that maps every digit from $1$ to $9$ to some (possibly the same) digit from $1$ to $9$.</p><p>You can perform the following operation <span class="tex-font-style-bf">no more than once</span>: choose a non-empty <span class="tex-font-style-bf">contiguous subsegment</span> of digits in $a$, and replace each digit $x$ from this segment with $f(x)$. For example, if $a = 1337$, $f(1) = 1$, $f(3) = 5$, $f(7) = 3$, and you choose the segment consisting of three rightmost digits, you get $1553$ as the result.</p><p>What is the maximum possible number you can obtain applying this operation no more than once?</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of digits in $a$.</p><p>The second line contains a string of $n$ characters, denoting the number $a$. Each character is a decimal digit from $1$ to $9$.</p><p>The third line contains exactly $9$ integers $f(1)$, $f(2)$, ..., $f(9)$ ($1 \le f(i) \le 9$).</p></div><div class="output-specification"><p>Print the maximum number you can get after applying the operation described in the statement no more than once.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of digits in $a$.</p><p>The second line contains a string of $n$ characters, denoting the number $a$. Each character is a decimal digit from $1$ to $9$.</p><p>The third line contains exactly $9$ integers $f(1)$, $f(2)$, ..., $f(9)$ ($1 \le f(i) \le 9$).</p>

## Output

<p>Print the maximum number you can get after applying the operation described in the statement no more than once.</p>





```input1
4
1337
1 2 5 4 6 6 3 1 9
```




```input2
5
11111
9 8 7 6 5 4 3 2 1
```




```input3
2
33
1 1 1 1 1 1 1 1 1
```




```output1
1557
```




```output2
99999
```




```output3
33
```


