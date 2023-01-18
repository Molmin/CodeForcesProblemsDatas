## Description

<div><p>Nikolay got a string $s$ of <span class="tex-font-style-bf">even</span> length $n$, which consists only of lowercase Latin letters '<span class="tex-font-style-tt">a</span>' and '<span class="tex-font-style-tt">b</span>'. Its positions are numbered from $1$ to $n$.</p><p>He wants to modify his string so that every its prefix of <span class="tex-font-style-bf">even</span> length has an equal amount of letters '<span class="tex-font-style-tt">a</span>' and '<span class="tex-font-style-tt">b</span>'. To achieve that, Nikolay can perform the following operation arbitrary number of times (possibly, zero): choose some position in his string and replace the letter on this position with the other letter (i.e. replace '<span class="tex-font-style-tt">a</span>' with '<span class="tex-font-style-tt">b</span>' or replace '<span class="tex-font-style-tt">b</span>' with '<span class="tex-font-style-tt">a</span>'). Nikolay can use no letters except '<span class="tex-font-style-tt">a</span>' and '<span class="tex-font-style-tt">b</span>'.</p><p>The prefix of string $s$ of length $l$ ($1 \le l \le n$) is a string $s[1..l]$.</p><p>For example, for the string $s=$"abba" there are two prefixes of the even length. The first is $s[1\dots2]=$"ab" and the second $s[1\dots4]=$"abba". Both of them have the same number of '<span class="tex-font-style-tt">a</span>' and '<span class="tex-font-style-tt">b</span>'.</p><p>Your task is to calculate the minimum number of operations Nikolay has to perform with the string $s$ to modify it so that every its prefix of <span class="tex-font-style-bf">even</span> length has an equal amount of letters '<span class="tex-font-style-tt">a</span>' and '<span class="tex-font-style-tt">b</span>'.</p></div><div class="input-specification"><p>The first line of the input contains one <span class="tex-font-style-bf">even</span> integer $n$ $(2 \le n \le 2\cdot10^{5})$ — the length of string $s$.</p><p>The second line of the input contains the string $s$ of length $n$, which consists only of lowercase Latin letters '<span class="tex-font-style-tt">a</span>' and '<span class="tex-font-style-tt">b</span>'.</p></div><div class="output-specification"><p>In the first line print the minimum number of operations Nikolay has to perform with the string $s$ to modify it so that every its prefix of <span class="tex-font-style-bf">even</span> length has an equal amount of letters '<span class="tex-font-style-tt">a</span>' and '<span class="tex-font-style-tt">b</span>'.</p><p>In the second line print the string Nikolay obtains after applying all the operations. If there are multiple answers, you can print any of them.</p></div>

## Input

<p>The first line of the input contains one <span class="tex-font-style-bf">even</span> integer $n$ $(2 \le n \le 2\cdot10^{5})$ — the length of string $s$.</p><p>The second line of the input contains the string $s$ of length $n$, which consists only of lowercase Latin letters '<span class="tex-font-style-tt">a</span>' and '<span class="tex-font-style-tt">b</span>'.</p>

## Output

<p>In the first line print the minimum number of operations Nikolay has to perform with the string $s$ to modify it so that every its prefix of <span class="tex-font-style-bf">even</span> length has an equal amount of letters '<span class="tex-font-style-tt">a</span>' and '<span class="tex-font-style-tt">b</span>'.</p><p>In the second line print the string Nikolay obtains after applying all the operations. If there are multiple answers, you can print any of them.</p>





```input1
4
bbbb
```




```input2
6
ababab
```




```input3
2
aa
```




```output1
2
abba
```




```output2
0
ababab
```




```output3
1
ba
```



## Note

<p>In the first example Nikolay has to perform two operations. For example, he can replace the first '<span class="tex-font-style-tt">b</span>' with '<span class="tex-font-style-tt">a</span>' and the last '<span class="tex-font-style-tt">b</span>' with '<span class="tex-font-style-tt">a</span>'. </p><p>In the second example Nikolay doesn't need to do anything because each prefix of an even length of the initial string already contains an equal amount of letters '<span class="tex-font-style-tt">a</span>' and '<span class="tex-font-style-tt">b</span>'.</p>
