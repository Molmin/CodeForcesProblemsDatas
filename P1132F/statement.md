## Description

<div><p>You are given a string $s$ of length $n$ consisting of lowercase Latin letters. You may apply some operations to this string: in one operation you can delete some contiguous substring of this string, if all letters in the substring you delete are equal. For example, after deleting substring <span class="tex-font-style-tt">bbbb</span> from string <span class="tex-font-style-tt">abbbbaccdd</span> we get the string <span class="tex-font-style-tt">aaccdd</span>.</p><p>Calculate the minimum number of operations to delete the whole string $s$.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 500$) — the length of string $s$.</p><p>The second line contains the string $s$ ($|s| = n$) consisting of lowercase Latin letters.</p></div><div class="output-specification"><p>Output a single integer — the minimal number of operation to delete string $s$.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 500$) — the length of string $s$.</p><p>The second line contains the string $s$ ($|s| = n$) consisting of lowercase Latin letters.</p>

## Output

<p>Output a single integer — the minimal number of operation to delete string $s$.</p>





```input1
5
abaca
```




```input2
8
abcddcba
```




```output1
3
```




```output2
4
```


