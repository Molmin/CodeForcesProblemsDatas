## Description

<div><p>Consider some set of distinct characters $A$ and some string $S$, consisting of exactly $n$ characters, where each character is present in $A$.</p><p>You are given an array of $m$ integers $b$ ($b_1 &lt; b_2 &lt; \dots &lt; b_m$). </p><p>You are allowed to perform the following move on the string $S$:</p><ol> <li> Choose some valid $i$ and set $k = b_i$; </li><li> Take the first $k$ characters of $S = Pr_k$; </li><li> Take the last $k$ characters of $S = Su_k$; </li><li> Substitute the first $k$ characters of $S$ with the reversed $Su_k$; </li><li> Substitute the last $k$ characters of $S$ with the reversed $Pr_k$. </li></ol><p>For example, let's take a look at $S =$ "<span class="tex-font-style-tt">abcdefghi</span>" and $k = 2$. $Pr_2 =$ "<span class="tex-font-style-tt">ab</span>", $Su_2 =$ "<span class="tex-font-style-tt">hi</span>". Reversed $Pr_2 =$ "<span class="tex-font-style-tt">ba</span>", $Su_2 =$ "<span class="tex-font-style-tt">ih</span>". Thus, the resulting $S$ is "<span class="tex-font-style-tt"><span class="tex-font-style-bf">ih</span>cdefg<span class="tex-font-style-bf">ba</span></span>".</p><p>The move can be performed arbitrary number of times (possibly zero). Any $i$ can be selected multiple times over these moves.</p><p>Let's call some strings $S$ and $T$ equal if and only if there exists such a sequence of moves to transmute string $S$ to string $T$. For the above example strings "<span class="tex-font-style-tt">abcdefghi</span>" and "<span class="tex-font-style-tt">ihcdefgba</span>" are equal. Also note that this implies $S = S$.</p><p>The task is simple. Count the number of distinct strings.</p><p>The answer can be huge enough, so calculate it modulo $998244353$.</p></div><div class="input-specification"><p>The first line contains three integers $n$, $m$ and $|A|$ ($2 \le n \le 10^9$, $1 \le m \le min(\frac n 2, 2 \cdot 10^5)$, $1 \le |A| \le 10^9$) — the length of the strings, the size of the array $b$ and the size of the set $A$, respectively.</p><p>The second line contains $m$ integers $b_1, b_2, \dots, b_m$ ($1 \le b_i \le \frac n 2$, $b_1 &lt; b_2 &lt; \dots &lt; b_m$).</p></div><div class="output-specification"><p>Print a single integer — the number of distinct strings of length $n$ with characters from set $A$ modulo $998244353$.</p></div>

## Input

<p>The first line contains three integers $n$, $m$ and $|A|$ ($2 \le n \le 10^9$, $1 \le m \le min(\frac n 2, 2 \cdot 10^5)$, $1 \le |A| \le 10^9$) — the length of the strings, the size of the array $b$ and the size of the set $A$, respectively.</p><p>The second line contains $m$ integers $b_1, b_2, \dots, b_m$ ($1 \le b_i \le \frac n 2$, $b_1 &lt; b_2 &lt; \dots &lt; b_m$).</p>

## Output

<p>Print a single integer — the number of distinct strings of length $n$ with characters from set $A$ modulo $998244353$.</p>





```input1
3 1 2
1

```




```input2
9 2 26
2 3

```




```input3
12 3 1
2 5 6

```




```output1
6

```




```output2
150352234

```




```output3
1

```



## Note

<p>Here are all the distinct strings for the first example. The chosen letters '<span class="tex-font-style-tt">a</span>' and '<span class="tex-font-style-tt">b</span>' are there just to show that the characters in $A$ are different. </p><ol> <li> "<span class="tex-font-style-tt">aaa</span>" </li><li> "<span class="tex-font-style-tt">aab</span>" = "<span class="tex-font-style-tt">baa</span>" </li><li> "<span class="tex-font-style-tt">aba</span>" </li><li> "<span class="tex-font-style-tt">abb</span>" = "<span class="tex-font-style-tt">bba</span>" </li><li> "<span class="tex-font-style-tt">bab</span>" </li><li> "<span class="tex-font-style-tt">bbb</span>" <ul></ul></li></ol>
