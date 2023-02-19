## Description

<div><p>Arkady owns a <span class="tex-font-style-bf">non-decreasing</span> array $a_1, a_2, \ldots, a_n$. You are jealous of its beauty and want to destroy this property. You have a so-called <span class="tex-font-style-it">XOR-gun</span> that you can use one or more times.</p><p>In one step you can select two <span class="tex-font-style-bf">consecutive</span> elements of the array, let's say $x$ and $y$, remove them from the array and insert the integer $x \oplus y$ on their place, where $\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>. Note that the length of the array decreases by one after the operation. You can't perform this operation when the length of the array reaches one.</p><p>For example, if the array is $[2, 5, 6, 8]$, you can select $5$ and $6$ and replace them with $5 \oplus 6 = 3$. The array becomes $[2, 3, 8]$.</p><p>You want the array no longer be non-decreasing. What is the minimum number of steps needed? If the array stays non-decreasing no matter what you do, print $-1$.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 10^5$)&nbsp;— the initial length of the array.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the elements of the array. It is guaranteed that $a_i \le a_{i + 1}$ for all $1 \le i &lt; n$.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the minimum number of steps needed. If there is no solution, print $-1$.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 10^5$)&nbsp;— the initial length of the array.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the elements of the array. It is guaranteed that $a_i \le a_{i + 1}$ for all $1 \le i &lt; n$.</p>

## Output

<p>Print a single integer&nbsp;— the minimum number of steps needed. If there is no solution, print $-1$.</p>





```input1
4
2 5 6 8
```




```input2
3
1 2 3
```




```input3
5
1 2 4 6 20
```




```output1
1
```




```output2
-1
```




```output3
2
```



## Note

<p>In the first example you can select $2$ and $5$ and the array becomes $[7, 6, 8]$.</p><p>In the second example you can only obtain arrays $[1, 1]$, $[3, 3]$ and $[0]$ which are all non-decreasing.</p><p>In the third example you can select $1$ and $2$ and the array becomes $[3, 4, 6, 20]$. Then you can, for example, select $3$ and $4$ and the array becomes $[7, 6, 20]$, which is no longer non-decreasing.</p>
