## Description

<div><p>Given 2 integers $u$ and $v$, find the shortest array such that <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise-xor</a> of its elements is $u$, and the sum of its elements is $v$.</p></div><div class="input-specification"><p>The only line contains 2 integers $u$ and $v$ $(0 \le u,v \le 10^{18})$.</p></div><div class="output-specification"><p>If there's no array that satisfies the condition, print "-1". Otherwise:</p><p>The first line should contain one integer, $n$, representing the length of the desired array. The next line should contain $n$ <span class="tex-font-style-bf">positive</span> integers, the array itself. If there are multiple possible answers, print any.</p></div>

## Input

<p>The only line contains 2 integers $u$ and $v$ $(0 \le u,v \le 10^{18})$.</p>

## Output

<p>If there's no array that satisfies the condition, print "-1". Otherwise:</p><p>The first line should contain one integer, $n$, representing the length of the desired array. The next line should contain $n$ <span class="tex-font-style-bf">positive</span> integers, the array itself. If there are multiple possible answers, print any.</p>





```input1
2 4
```




```input2
1 3
```




```input3
8 5
```




```input4
0 0
```




```output1
2
3 1
```




```output2
3
1 1 1
```




```output3
-1
```




```output4
0
```



## Note

<p>In the first sample, $3\oplus 1 = 2$ and $3 + 1 = 4$. There is no valid array of smaller length.</p><p>Notice that in the fourth sample the array is empty.</p>
