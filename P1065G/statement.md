## Description

<div><p>Let's denote (yet again) the sequence of Fibonacci strings:</p><p>$F(0) = $ <span class="tex-font-style-tt">0</span>, $F(1) = $ <span class="tex-font-style-tt">1</span>, $F(i) = F(i - 2) + F(i - 1)$, where the plus sign denotes the concatenation of two strings.</p><p>Let's denote the <span class="tex-font-style-bf">lexicographically sorted</span> sequence of suffixes of string $F(i)$ as $A(F(i))$. For example, $F(4)$ is <span class="tex-font-style-tt">01101</span>, and $A(F(4))$ is the following sequence: <span class="tex-font-style-tt">01</span>, <span class="tex-font-style-tt">01101</span>, <span class="tex-font-style-tt">1</span>, <span class="tex-font-style-tt">101</span>, <span class="tex-font-style-tt">1101</span>. Elements in this sequence are numbered from $1$.</p><p>Your task is to print $m$ first characters of $k$-th element of $A(F(n))$. If there are less than $m$ characters in this suffix, then output the whole suffix.</p></div><div class="input-specification"><p>The only line of the input contains three numbers $n$, $k$ and $m$ ($1 \le n, m \le 200$, $1 \le k \le 10^{18}$) denoting the index of the Fibonacci string you have to consider, the index of the element of $A(F(n))$ and the number of characters you have to output, respectively.</p><p>It is guaranteed that $k$ does not exceed the length of $F(n)$.</p></div><div class="output-specification"><p>Output $m$ first characters of $k$-th element of $A(F(n))$, or the whole element if its length is less than $m$.</p></div>

## Input

<p>The only line of the input contains three numbers $n$, $k$ and $m$ ($1 \le n, m \le 200$, $1 \le k \le 10^{18}$) denoting the index of the Fibonacci string you have to consider, the index of the element of $A(F(n))$ and the number of characters you have to output, respectively.</p><p>It is guaranteed that $k$ does not exceed the length of $F(n)$.</p>

## Output

<p>Output $m$ first characters of $k$-th element of $A(F(n))$, or the whole element if its length is less than $m$.</p>





```input1
4 5 3

```




```input2
4 3 3

```




```output1
110

```




```output2
1

```


