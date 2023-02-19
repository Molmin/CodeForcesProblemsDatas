## Description

<div><p>Now you get Baby Ehab's first words: "Given an integer $n$, find the longest subsequence of $[1,2, \ldots, n-1]$ whose product is $1$ modulo $n$." Please solve the problem.</p><p>A sequence $b$ is a subsequence of an array $a$ if $b$ can be obtained from $a$ by deleting some (possibly all) elements. The product of an empty subsequence is equal to $1$.</p></div><div class="input-specification"><p>The only line contains the integer $n$ ($2 \le n \le 10^5$).</p></div><div class="output-specification"><p>The first line should contain a single integer, the length of the longest subsequence.</p><p>The second line should contain the elements of the subsequence, <span class="tex-font-style-bf">in increasing order</span>.</p><p>If there are multiple solutions, you can print any.</p></div>

## Input

<p>The only line contains the integer $n$ ($2 \le n \le 10^5$).</p>

## Output

<p>The first line should contain a single integer, the length of the longest subsequence.</p><p>The second line should contain the elements of the subsequence, <span class="tex-font-style-bf">in increasing order</span>.</p><p>If there are multiple solutions, you can print any.</p>





```input1
5
```




```input2
8
```




```output1
3
1 2 3
```




```output2
4
1 3 5 7
```



## Note

<p>In the first example, the product of the elements is $6$ which is congruent to $1$ modulo $5$. The only longer subsequence is $[1,2,3,4]$. Its product is $24$ which is congruent to $4$ modulo $5$. Hence, the answer is $[1,2,3]$.</p>
