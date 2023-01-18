## Description

<div><p>You are given two strings $s$ and $t$ <span class="tex-font-style-bf">both of length $2$</span> and both consisting only of characters '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>' and '<span class="tex-font-style-tt">c</span>'.</p><p>Possible examples of strings $s$ and $t$: "<span class="tex-font-style-tt">ab</span>", "<span class="tex-font-style-tt">ca</span>", "<span class="tex-font-style-tt">bb</span>".</p><p>You have to find a string $res$ consisting of $3n$ characters, $n$ characters should be '<span class="tex-font-style-tt">a</span>', $n$ characters should be '<span class="tex-font-style-tt">b</span>' and $n$ characters should be '<span class="tex-font-style-tt">c</span>' and $s$ and $t$ should not occur in $res$ as substrings.</p><p>A substring of a string is a contiguous subsequence of that string. So, the strings "<span class="tex-font-style-tt">ab</span>", "<span class="tex-font-style-tt">ac</span>" and "<span class="tex-font-style-tt">cc</span>" are substrings of the string "<span class="tex-font-style-tt">abacc</span>", but the strings "<span class="tex-font-style-tt">bc</span>", "<span class="tex-font-style-tt">aa</span>" and "<span class="tex-font-style-tt">cb</span>" are not substrings of the string "<span class="tex-font-style-tt">abacc</span>".</p><p>If there are multiple answers, you can print any of them.</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($1 \le n \le 10^5$) — the number of characters '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>' and '<span class="tex-font-style-tt">c</span>' in the resulting string.</p><p>The second line of the input contains one string $s$ of length $2$ consisting of characters '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>' and '<span class="tex-font-style-tt">c</span>'.</p><p>The third line of the input contains one string $t$ of length $2$ consisting of characters '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>' and '<span class="tex-font-style-tt">c</span>'.</p></div><div class="output-specification"><p>If it is impossible to find the suitable string, print "<span class="tex-font-style-tt">NO</span>" on the first line. </p><p>Otherwise print "<span class="tex-font-style-tt">YES</span>" on the first line and string $res$ on the second line. $res$ should consist of $3n$ characters, $n$ characters should be '<span class="tex-font-style-tt">a</span>', $n$ characters should be '<span class="tex-font-style-tt">b</span>' and $n$ characters should be '<span class="tex-font-style-tt">c</span>' and $s$ and $t$ should not occur in $res$ as substrings.</p><p>If there are multiple answers, you can print any of them.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($1 \le n \le 10^5$) — the number of characters '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>' and '<span class="tex-font-style-tt">c</span>' in the resulting string.</p><p>The second line of the input contains one string $s$ of length $2$ consisting of characters '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>' and '<span class="tex-font-style-tt">c</span>'.</p><p>The third line of the input contains one string $t$ of length $2$ consisting of characters '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>' and '<span class="tex-font-style-tt">c</span>'.</p>

## Output

<p>If it is impossible to find the suitable string, print "<span class="tex-font-style-tt">NO</span>" on the first line. </p><p>Otherwise print "<span class="tex-font-style-tt">YES</span>" on the first line and string $res$ on the second line. $res$ should consist of $3n$ characters, $n$ characters should be '<span class="tex-font-style-tt">a</span>', $n$ characters should be '<span class="tex-font-style-tt">b</span>' and $n$ characters should be '<span class="tex-font-style-tt">c</span>' and $s$ and $t$ should not occur in $res$ as substrings.</p><p>If there are multiple answers, you can print any of them.</p>





```input1
2
ab
bc
```




```input2
3
aa
bc
```




```input3
1
cb
ac
```




```output1
YES
acbbac
```




```output2
YES
cacbacbab
```




```output3
YES
abc
```


