## Description

<div><p>Currently, XXOC's rap is a string consisting of zeroes, ones, and question marks. Unfortunately, haters gonna hate. They will write $x$ angry comments for every occurrence of <span class="tex-font-style-bf">subsequence</span> <span class="tex-font-style-tt">01</span> and $y$ angry comments for every occurrence of <span class="tex-font-style-bf">subsequence</span> <span class="tex-font-style-tt">10</span>. You should replace all the question marks with <span class="tex-font-style-tt">0</span> or <span class="tex-font-style-tt">1</span> in such a way that the number of angry comments would be as small as possible.</p><p>String $b$ is a subsequence of string $a$, if it can be obtained by removing some characters from $a$. Two occurrences of a subsequence are considered distinct if sets of positions of remaining characters are distinct.</p></div><div class="input-specification"><p>The first line contains string $s$&nbsp;— XXOC's rap ($1 \le |s| \leq 10^5$). The second line contains two integers $x$ and $y$&nbsp;— the number of angry comments XXOC will recieve for every occurrence of <span class="tex-font-style-tt">01</span> and <span class="tex-font-style-tt">10</span> accordingly ($0 \leq x, y \leq 10^6$).</p></div><div class="output-specification"><p>Output a single integer&nbsp;— the minimum number of angry comments.</p></div>

## Input

<p>The first line contains string $s$&nbsp;— XXOC's rap ($1 \le |s| \leq 10^5$). The second line contains two integers $x$ and $y$&nbsp;— the number of angry comments XXOC will recieve for every occurrence of <span class="tex-font-style-tt">01</span> and <span class="tex-font-style-tt">10</span> accordingly ($0 \leq x, y \leq 10^6$).</p>

## Output

<p>Output a single integer&nbsp;— the minimum number of angry comments.</p>





```input1
0?1
2 3
```




```input2
?????
13 37
```




```input3
?10?
239 7
```




```input4
01101001
5 7
```




```output1
4
```




```output2
0
```




```output3
28
```




```output4
96
```



## Note

<p>In the first example one of the optimum ways to replace is <span class="tex-font-style-tt">001</span>. Then there will be $2$ subsequences <span class="tex-font-style-tt">01</span> and $0$ subsequences <span class="tex-font-style-tt">10</span>. Total number of angry comments will be equal to $2 \cdot 2 + 0 \cdot 3 = 4$.</p><p>In the second example one of the optimum ways to replace is <span class="tex-font-style-tt">11111</span>. Then there will be $0$ subsequences <span class="tex-font-style-tt">01</span> and $0$ subsequences <span class="tex-font-style-tt">10</span>. Total number of angry comments will be equal to $0 \cdot 13 + 0 \cdot 37 = 0$.</p><p>In the third example one of the optimum ways to replace is <span class="tex-font-style-tt">1100</span>. Then there will be $0$ subsequences <span class="tex-font-style-tt">01</span> and $4$ subsequences <span class="tex-font-style-tt">10</span>. Total number of angry comments will be equal to $0 \cdot 239 + 4 \cdot 7 = 28$.</p><p>In the fourth example one of the optimum ways to replace is <span class="tex-font-style-tt">01101001</span>. Then there will be $8$ subsequences <span class="tex-font-style-tt">01</span> and $8$ subsequences <span class="tex-font-style-tt">10</span>. Total number of angry comments will be equal to $8 \cdot 5 + 8 \cdot 7 = 96$.</p>
