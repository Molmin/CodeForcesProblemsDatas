## Description

<div><p>Vasya has got an array consisting of $n$ integers, and two integers $k$ and $len$ in addition. All numbers in the array are either between $1$ and $k$ (inclusive), or equal to $-1$. The array is good if there is no segment of $len$ consecutive <span class="tex-font-style-bf">equal</span> numbers.</p><p>Vasya will replace each $-1$ with some number from $1$ to $k$ (inclusive) in such a way that the resulting array is good. Tell him the number of ways to do this replacement. Since the answer may be large, print it modulo $998244353$.</p></div><div class="input-specification"><p>The first line contains three integers $n, k$ and $len$ ($1 \le n \le 10^5, 1 \le k \le 100, 1 \le len \le n$).</p><p>The second line contains $n$ numbers — the array. Each number is either $-1$ or between $1$ and $k$ (inclusive).</p></div><div class="output-specification"><p>Print one integer — the number of ways to replace each $-1$ with some number from $1$ to $k$ (inclusive) so the array is good. The answer may be large, so print it modulo $998244353$.</p></div>

## Input

<p>The first line contains three integers $n, k$ and $len$ ($1 \le n \le 10^5, 1 \le k \le 100, 1 \le len \le n$).</p><p>The second line contains $n$ numbers — the array. Each number is either $-1$ or between $1$ and $k$ (inclusive).</p>

## Output

<p>Print one integer — the number of ways to replace each $-1$ with some number from $1$ to $k$ (inclusive) so the array is good. The answer may be large, so print it modulo $998244353$.</p>





```input1
5 2 3
1 -1 1 -1 2
```




```input2
6 3 2
1 1 -1 -1 -1 -1
```




```input3
10 42 7
-1 -1 -1 -1 -1 -1 -1 -1 -1 -1
```




```output1
2
```




```output2
0
```




```output3
645711643
```



## Note

<p>Possible answers in the first test: </p><ol> <li> $[1, 2, 1, 1, 2]$; </li><li> $[1, 2, 1, 2, 2]$. </li></ol><p>There is no way to make the array good in the second test, since first two elements are equal.</p><p>There are too many answers in the third test, so we won't describe any of them.</p>
