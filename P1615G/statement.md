## Description

<div><p>You are given an array $a$ consisting of $n$ non-negative integers.</p><p>You have to replace each $0$ in $a$ with an integer from $1$ to $n$ (different elements equal to $0$ can be replaced by different integers).</p><p>The <span class="tex-font-style-it">value</span> of the array you obtain is the number of integers $k$ from $1$ to $n$ such that the following condition holds: there exist a pair of adjacent elements equal to $k$ (i. e. there exists some $i \in [1, n - 1]$ such that $a_i = a_{i + 1} = k$). If there are multiple such pairs for some integer $k$, this integer is counted in the <span class="tex-font-style-it">value</span> only once.</p><p>Your task is to obtain the array with the maximum possible <span class="tex-font-style-it">value</span>.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($2 \le n \le 3 \cdot 10^5$)&nbsp;— the number of elements in the array.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le \min(n, 600)$)&nbsp;— the elements of the array.</p></div><div class="output-specification"><p>Print $n$ integers not less than $1$ and not greater than $n$&nbsp;— the array with the maximum possible <span class="tex-font-style-it">value</span> you can obtain.</p><p>If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains one integer $n$ ($2 \le n \le 3 \cdot 10^5$)&nbsp;— the number of elements in the array.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le \min(n, 600)$)&nbsp;— the elements of the array.</p>

## Output

<p>Print $n$ integers not less than $1$ and not greater than $n$&nbsp;— the array with the maximum possible <span class="tex-font-style-it">value</span> you can obtain.</p><p>If there are multiple answers, print any of them.</p>





```input1
4
1 1 0 2
```




```input2
5
0 0 0 0 0
```




```input3
5
1 2 3 4 5
```




```input4
6
1 0 0 0 0 1
```




```input5
3
3 0 2
```




```input6
5
1 0 2 0 1
```




```input7
7
1 0 2 3 1 0 2
```




```output1
1 1 2 2
```




```output2
3 1 1 3 3
```




```output3
1 2 3 4 5
```




```output4
1 2 3 3 1 1
```




```output5
3 2 2
```




```output6
1 2 2 1 1
```




```output7
1 2 2 3 1 1 2
```


