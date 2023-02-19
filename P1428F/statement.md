## Description

<div><p>Zookeeper is buying a carton of fruit to feed his pet wabbit. The fruits are a sequence of apples and oranges, which is represented by a binary string $s_1s_2\ldots s_n$ of length $n$. $1$ represents an apple and $0$ represents an orange.</p><p>Since wabbit is allergic to eating oranges, Zookeeper would like to find the longest <span class="tex-font-style-bf">contiguous</span> sequence of apples. Let $f(l,r)$ be the longest <span class="tex-font-style-bf">contiguous</span> sequence of apples in the substring $s_{l}s_{l+1}\ldots s_{r}$. </p><p>Help Zookeeper find $\sum_{l=1}^{n} \sum_{r=l}^{n} f(l,r)$, or the sum of $f$ across all substrings.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ $(1 \leq n \leq 5 \cdot 10^5)$.</p><p> The next line contains a binary string $s$ of length $n$ $(s_i \in \{0,1\})$ </p></div><div class="output-specification"><p>Print a single integer: $\sum_{l=1}^{n} \sum_{r=l}^{n} f(l,r)$. </p></div>

## Input

<p>The first line contains a single integer $n$ $(1 \leq n \leq 5 \cdot 10^5)$.</p><p> The next line contains a binary string $s$ of length $n$ $(s_i \in \{0,1\})$ </p>

## Output

<p>Print a single integer: $\sum_{l=1}^{n} \sum_{r=l}^{n} f(l,r)$. </p>





```input1
4
0110
```




```input2
7
1101001
```




```input3
12
011100011100
```




```output1
12
```




```output2
30
```




```output3
156
```



## Note

<p>In the first test, there are ten substrings. The list of them (we let $[l,r]$ be the substring $s_l s_{l+1} \ldots s_r$):</p><ul> <li> $[1,1]$: 0 </li><li> $[1,2]$: 01 </li><li> $[1,3]$: 011 </li><li> $[1,4]$: 0110 </li><li> $[2,2]$: 1 </li><li> $[2,3]$: 11 </li><li> $[2,4]$: 110 </li><li> $[3,3]$: 1 </li><li> $[3,4]$: 10 </li><li> $[4,4]$: 0 </li></ul><p>The lengths of the longest contiguous sequence of ones in each of these ten substrings are $0,1,2,2,1,2,2,1,1,0$ respectively. Hence, the answer is $0+1+2+2+1+2+2+1+1+0 = 12$.</p>
