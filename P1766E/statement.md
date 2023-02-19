## Description

<div><p>For a sequence of integers $[x_1, x_2, \dots, x_k]$, let's define its <span class="tex-font-style-it">decomposition</span> as follows:</p><p>Process the sequence from the first element to the last one, maintaining the list of its subsequences. When you process the element $x_i$, append it to the end of the <span class="tex-font-style-bf">first</span> subsequence in the list such that the bitwise AND of its last element and $x_i$ is greater than $0$. If there is no such subsequence in the list, create a new subsequence with only one element $x_i$ and append it to the end of the list of subsequences.</p><p>For example, let's analyze the decomposition of the sequence $[1, 3, 2, 0, 1, 3, 2, 1]$:</p><ul> <li> processing element $1$, the list of subsequences is empty. There is no subsequence to append $1$ to, so we create a new subsequence $[1]$; </li><li> processing element $3$, the list of subsequences is $[[1]]$. Since the bitwise AND of $3$ and $1$ is $1$, the element is appended to the first subsequence; </li><li> processing element $2$, the list of subsequences is $[[1, 3]]$. Since the bitwise AND of $2$ and $3$ is $2$, the element is appended to the first subsequence; </li><li> processing element $0$, the list of subsequences is $[[1, 3, 2]]$. There is no subsequence to append $0$ to, so we create a new subsequence $[0]$; </li><li> processing element $1$, the list of subsequences is $[[1, 3, 2], [0]]$. There is no subsequence to append $1$ to, so we create a new subsequence $[1]$; </li><li> processing element $3$, the list of subsequences is $[[1, 3, 2], [0], [1]]$. Since the bitwise AND of $3$ and $2$ is $2$, the element is appended to the first subsequence; </li><li> processing element $2$, the list of subsequences is $[[1, 3, 2, 3], [0], [1]]$. Since the bitwise AND of $2$ and $3$ is $2$, the element is appended to the first subsequence; </li><li> processing element $1$, the list of subsequences is $[[1, 3, 2, 3, 2], [0], [1]]$. The element $1$ cannot be appended to any of the first two subsequences, but can be appended to the third one. </li></ul><p>The resulting list of subsequences is $[[1, 3, 2, 3, 2], [0], [1, 1]]$.</p><p>Let $f([x_1, x_2, \dots, x_k])$ be the number of subsequences the sequence $[x_1, x_2, \dots, x_k]$ is decomposed into.</p><p><span class="tex-font-style-it">Now, for the problem itself</span>.</p><p>You are given a sequence $[a_1, a_2, \dots, a_n]$, where each element is an integer from $0$ to $3$. Let $a[i..j]$ be the sequence $[a_i, a_{i+1}, \dots, a_j]$. You have to calculate $\sum \limits_{i=1}^n \sum \limits_{j=i}^n f(a[i..j])$.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 3 \cdot 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 3$).</p></div><div class="output-specification"><p>Print one integer, which should be equal to $\sum \limits_{i=1}^n \sum \limits_{j=i}^n f(a[i..j])$.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 3 \cdot 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 3$).</p>

## Output

<p>Print one integer, which should be equal to $\sum \limits_{i=1}^n \sum \limits_{j=i}^n f(a[i..j])$.</p>





```input1
8
1 3 2 0 1 3 2 1
```




```input2
5
0 0 0 0 0
```




```output1
71
```




```output2
35
```


