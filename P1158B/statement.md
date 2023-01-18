## Description

<div><p>Let $s$ be some string consisting of symbols "<span class="tex-font-style-tt">0</span>" or "<span class="tex-font-style-tt">1</span>". Let's call a string $t$ a substring of string $s$, if there exists such number $1 \leq l \leq |s| - |t| + 1$ that $t = s_l s_{l+1} \ldots s_{l + |t| - 1}$. Let's call a substring $t$ of string $s$ unique, if there exist only one such $l$. </p><p>For example, let $s = $"<span class="tex-font-style-tt">1010111</span>". A string $t = $"<span class="tex-font-style-tt">010</span>" is an unique substring of $s$, because $l = 2$ is the only one suitable number. But, for example $t = $"<span class="tex-font-style-tt">10</span>" isn't a unique substring of $s$, because $l = 1$ and $l = 3$ are suitable. And for example $t =$"<span class="tex-font-style-tt">00</span>" at all isn't a substring of $s$, because there is no suitable $l$.</p><p>Today Vasya solved the following problem at the informatics lesson: given a string consisting of symbols "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">1</span>", the task is to find the length of its minimal unique substring. He has written a solution to this problem and wants to test it. He is asking you to help him.</p><p>You are given $2$ positive integers $n$ and $k$, such that $(n \bmod 2) = (k \bmod 2)$, where $(x \bmod 2)$ is operation of taking remainder of $x$ by dividing on $2$. Find any string $s$ consisting of $n$ symbols "<span class="tex-font-style-tt">0</span>" or "<span class="tex-font-style-tt">1</span>", such that the length of its minimal unique substring is equal to $k$.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$, separated by spaces ($1 \leq k \leq n \leq 100\,000$, $(k \bmod 2) = (n \bmod 2)$).</p></div><div class="output-specification"><p>Print a string $s$ of length $n$, consisting of symbols "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">1</span>". Minimal length of the unique substring of $s$ should be equal to $k$. You can find <span class="tex-font-style-bf">any</span> suitable string. It is guaranteed, that there exists at least one such string.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$, separated by spaces ($1 \leq k \leq n \leq 100\,000$, $(k \bmod 2) = (n \bmod 2)$).</p>

## Output

<p>Print a string $s$ of length $n$, consisting of symbols "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">1</span>". Minimal length of the unique substring of $s$ should be equal to $k$. You can find <span class="tex-font-style-bf">any</span> suitable string. It is guaranteed, that there exists at least one such string.</p>





```input1
4 4
```




```input2
5 3
```




```input3
7 3
```




```output1
1111
```




```output2
01010
```




```output3
1011011
```



## Note

<p>In the first test, it's easy to see, that the only unique substring of string $s = $"<span class="tex-font-style-tt">1111</span>" is all string $s$, which has length $4$.</p><p>In the second test a string $s = $"<span class="tex-font-style-tt">01010</span>" has minimal unique substring $t =$"<span class="tex-font-style-tt">101</span>", which has length $3$.</p><p>In the third test a string $s = $"<span class="tex-font-style-tt">1011011</span>" has minimal unique substring $t =$"<span class="tex-font-style-tt">110</span>", which has length $3$.</p>
