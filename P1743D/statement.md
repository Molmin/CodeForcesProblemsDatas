## Description

<div><p>You are given a string $s$ consisting of $n$ characters. Each character of $s$ is either <span class="tex-font-style-tt">0</span> or <span class="tex-font-style-tt">1</span>.</p><p>A substring of $s$ is a contiguous subsequence of its characters.</p><p>You have to choose two substrings of $s$ (possibly intersecting, possibly the same, possibly non-intersecting — just any two substrings). After choosing them, you calculate the value of the chosen pair of substrings as follows:</p><ul> <li> let $s_1$ be the first substring, $s_2$ be the second chosen substring, and $f(s_i)$ be the integer such that $s_i$ is its binary representation (for example, if $s_i$ is <span class="tex-font-style-tt">11010</span>, $f(s_i) = 26$); </li><li> the value is the <span class="tex-font-style-bf">bitwise OR</span> of $f(s_1)$ and $f(s_2)$. </li></ul><p>Calculate the maximum possible value you can get, and print it <span class="tex-font-style-bf">in binary representation without leading zeroes</span>.</p></div><div class="input-specification"><p>The first line contains one integer $n$ — the number of characters in $s$.</p><p>The second line contains $s$ itself, consisting of exactly $n$ characters <span class="tex-font-style-tt">0</span> and/or <span class="tex-font-style-tt">1</span>.</p><p><span class="tex-font-style-bf">All non-example tests in this problem are generated randomly: every character of $s$ is chosen independently of other characters; for each character, the probability of it being <span class="tex-font-style-tt">1</span> is exactly $\frac{1}{2}$</span>.</p><p>This problem has exactly $40$ tests. Tests from $1$ to $3$ are the examples; tests from $4$ to $40$ are generated randomly. In tests from $4$ to $10$, $n = 5$; in tests from $11$ to $20$, $n = 1000$; in tests from $21$ to $40$, $n = 10^6$. </p><p><span class="tex-font-style-bf">Hacks are forbidden in this problem.</span></p></div><div class="output-specification"><p>Print the maximum possible value you can get <span class="tex-font-style-bf">in binary representation without leading zeroes</span>.</p></div>

## Input

<p>The first line contains one integer $n$ — the number of characters in $s$.</p><p>The second line contains $s$ itself, consisting of exactly $n$ characters <span class="tex-font-style-tt">0</span> and/or <span class="tex-font-style-tt">1</span>.</p><p><span class="tex-font-style-bf">All non-example tests in this problem are generated randomly: every character of $s$ is chosen independently of other characters; for each character, the probability of it being <span class="tex-font-style-tt">1</span> is exactly $\frac{1}{2}$</span>.</p><p>This problem has exactly $40$ tests. Tests from $1$ to $3$ are the examples; tests from $4$ to $40$ are generated randomly. In tests from $4$ to $10$, $n = 5$; in tests from $11$ to $20$, $n = 1000$; in tests from $21$ to $40$, $n = 10^6$. </p><p><span class="tex-font-style-bf">Hacks are forbidden in this problem.</span></p>

## Output

<p>Print the maximum possible value you can get <span class="tex-font-style-bf">in binary representation without leading zeroes</span>.</p>





```input1
5
11010
```




```input2
7
1110010
```




```input3
4
0000
```




```output1
11111
```




```output2
1111110
```




```output3
0
```



## Note

<p>In the first example, you can choose the substrings <span class="tex-font-style-tt">11010</span> and <span class="tex-font-style-tt">101</span>. $f(s_1) = 26$, $f(s_2) = 5$, their bitwise OR is $31$, and the binary representation of $31$ is <span class="tex-font-style-tt">11111</span>.</p><p>In the second example, you can choose the substrings <span class="tex-font-style-tt">1110010</span> and <span class="tex-font-style-tt">11100</span>.</p>
