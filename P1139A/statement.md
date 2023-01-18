## Description

<div><p>You are given a string $s=s_1s_2\dots s_n$ of length $n$, which only contains digits $1$, $2$, ..., $9$.</p><p>A substring $s[l \dots r]$ of $s$ is a string $s_l s_{l + 1} s_{l + 2} \ldots s_r$. A substring $s[l \dots r]$ of $s$ is called <span class="tex-font-style-it">even</span> if the number represented by it is even. </p><p>Find the number of even substrings of $s$. Note, that even if some substrings are equal as strings, but have different $l$ and $r$, they are counted as <span class="tex-font-style-bf">different</span> substrings.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($1 \le n \le 65000$)&nbsp;— the length of the string $s$.</p><p>The second line contains a string $s$ of length $n$. The string $s$ consists only of digits $1$, $2$, ..., $9$.</p></div><div class="output-specification"><p>Print the number of even substrings of $s$.</p></div>

## Input

<p>The first line contains an integer $n$ ($1 \le n \le 65000$)&nbsp;— the length of the string $s$.</p><p>The second line contains a string $s$ of length $n$. The string $s$ consists only of digits $1$, $2$, ..., $9$.</p>

## Output

<p>Print the number of even substrings of $s$.</p>





```input1
4
1234
```




```input2
4
2244
```




```output1
6
```




```output2
10
```



## Note

<p>In the first example, the $[l, r]$ pairs corresponding to even substrings are: </p><ul> <li> $s[1 \dots 2]$</li><li> $s[2 \dots 2]$</li><li> $s[1 \dots 4]$</li><li> $s[2 \dots 4]$</li><li> $s[3 \dots 4]$</li><li> $s[4 \dots 4]$ </li></ul><p>In the second example, all $10$ substrings of $s$ are even substrings. Note, that while substrings $s[1 \dots 1]$ and $s[2 \dots 2]$ both define the substring "<span class="tex-font-style-tt">2</span>", they are still counted as different substrings.</p>
