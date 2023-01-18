## Description

<div><p>Polycarp likes arithmetic progressions. A sequence $[a_1, a_2, \dots, a_n]$ is called an arithmetic progression if for each $i$ ($1 \le i &lt; n$) the value $a_{i+1} - a_i$ is the same. For example, the sequences $[42]$, $[5, 5, 5]$, $[2, 11, 20, 29]$ and $[3, 2, 1, 0]$ are arithmetic progressions, but $[1, 0, 1]$, $[1, 3, 9]$ and $[2, 3, 1]$ are not.</p><p>It follows from the definition that any sequence of length one or two is an arithmetic progression.</p><p>Polycarp found some sequence of positive integers $[b_1, b_2, \dots, b_n]$. He agrees to change each element by at most one. In the other words, for each element there are exactly three options: an element can be decreased by $1$, an element can be increased by $1$, an element can be left unchanged.</p><p>Determine a minimum possible number of elements in $b$ which can be changed (by exactly one), so that the sequence $b$ becomes an arithmetic progression, or report that it is impossible.</p><p>It is possible that the resulting sequence contains element equals $0$.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ $(1 \le n \le 100\,000)$ — the number of elements in $b$.</p><p>The second line contains a sequence $b_1, b_2, \dots, b_n$ $(1 \le b_i \le 10^{9})$.</p></div><div class="output-specification"><p>If it is impossible to make an arithmetic progression with described operations, print <span class="tex-font-style-tt">-1</span>. In the other case, print non-negative integer — the minimum number of elements to change to make the given sequence becomes an arithmetic progression. The only allowed operation is to add/to subtract one from an element (can't use operation twice to the same position).</p></div>

## Input

<p>The first line contains a single integer $n$ $(1 \le n \le 100\,000)$ — the number of elements in $b$.</p><p>The second line contains a sequence $b_1, b_2, \dots, b_n$ $(1 \le b_i \le 10^{9})$.</p>

## Output

<p>If it is impossible to make an arithmetic progression with described operations, print <span class="tex-font-style-tt">-1</span>. In the other case, print non-negative integer — the minimum number of elements to change to make the given sequence becomes an arithmetic progression. The only allowed operation is to add/to subtract one from an element (can't use operation twice to the same position).</p>





```input1
4
24 21 14 10

```




```input2
2
500 500

```




```input3
3
14 5 1

```




```input4
5
1 3 6 9 12

```




```output1
3

```




```output2
0

```




```output3
-1

```




```output4
1

```



## Note

<p>In the first example Polycarp should increase the first number on $1$, decrease the second number on $1$, increase the third number on $1$, and the fourth number should left unchanged. So, after Polycarp changed three elements by one, his sequence became equals to $[25, 20, 15, 10]$, which is an arithmetic progression.</p><p>In the second example Polycarp should not change anything, because his sequence is an arithmetic progression.</p><p>In the third example it is impossible to make an arithmetic progression.</p><p>In the fourth example Polycarp should change only the first element, he should decrease it on one. After that his sequence will looks like $[0, 3, 6, 9, 12]$, which is an arithmetic progression.</p>
