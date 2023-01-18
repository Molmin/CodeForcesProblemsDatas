## Description

<div><p>You are given a binary string $s$.</p><p>Find the number of distinct <span class="tex-font-style-it">cyclical</span> binary strings of length $n$ which contain $s$ as a substring.</p><p>The cyclical string $t$ contains $s$ as a substring if there is some cyclical shift of string $t$, such that $s$ is a substring of this cyclical shift of $t$.</p><p>For example, the cyclical string "<span class="tex-font-style-tt">000111</span>" contains substrings "<span class="tex-font-style-tt">001</span>", "<span class="tex-font-style-tt">01110</span>" and "<span class="tex-font-style-tt">10</span>", but doesn't contain "<span class="tex-font-style-tt">0110</span>" and "<span class="tex-font-style-tt">10110</span>".</p><p>Two cyclical strings are called different if they differ from each other as strings. For example, two different strings, which differ from each other by a cyclical shift, are still considered <span class="tex-font-style-bf">different</span> cyclical strings.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 40$)&nbsp;— the length of the target string $t$.</p><p>The next line contains the string $s$ ($1 \le |s| \le n$)&nbsp;— the string which must be a substring of cyclical string $t$. String $s$ contains only characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>'.</p></div><div class="output-specification"><p>Print the only integer&nbsp;— the number of distinct cyclical binary strings $t$, which contain $s$ as a substring.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 40$)&nbsp;— the length of the target string $t$.</p><p>The next line contains the string $s$ ($1 \le |s| \le n$)&nbsp;— the string which must be a substring of cyclical string $t$. String $s$ contains only characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>'.</p>

## Output

<p>Print the only integer&nbsp;— the number of distinct cyclical binary strings $t$, which contain $s$ as a substring.</p>





```input1
2
0

```




```input2
4
1010

```




```input3
20
10101010101010

```




```output1
3
```




```output2
2
```




```output3
962
```



## Note

<p>In the first example, there are three cyclical strings, which contain "<span class="tex-font-style-tt">0</span>"&nbsp;— "<span class="tex-font-style-tt">00</span>", "<span class="tex-font-style-tt">01</span>" and "<span class="tex-font-style-tt">10</span>".</p><p>In the second example, there are only two such strings&nbsp;— "<span class="tex-font-style-tt">1010</span>", "<span class="tex-font-style-tt">0101</span>".</p>
