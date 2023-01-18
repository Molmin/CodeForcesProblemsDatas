## Description

<div><p>You are given a string $s$ consisting of exactly $n$ characters, and each character is either '<span class="tex-font-style-tt">0</span>', '<span class="tex-font-style-tt">1</span>' or '<span class="tex-font-style-tt">2</span>'. Such strings are called <span class="tex-font-style-bf">ternary strings</span>.</p><p>Your task is to <span class="tex-font-style-bf">replace minimum number of characters</span> in this string with other characters to obtain a <span class="tex-font-style-it">balanced</span> ternary string (<span class="tex-font-style-it">balanced</span> ternary string is a ternary string such that the number of characters '<span class="tex-font-style-tt">0</span>' in this string is equal to the number of characters '<span class="tex-font-style-tt">1</span>', and the number of characters '<span class="tex-font-style-tt">1</span>' (and '<span class="tex-font-style-tt">0</span>' obviously) is equal to the number of characters '<span class="tex-font-style-tt">2</span>').</p><p>Among all possible <span class="tex-font-style-it">balanced</span> ternary strings you have to obtain the lexicographically (alphabetically) smallest.</p><p>Note that you can neither remove characters from the string nor add characters to the string. Also note that you can replace the given characters only with characters '<span class="tex-font-style-tt">0</span>', '<span class="tex-font-style-tt">1</span>' and '<span class="tex-font-style-tt">2</span>'.</p><p>It is <span class="tex-font-style-bf">guaranteed</span> that the answer exists.</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($3 \le n \le 3 \cdot 10^5$, $n$ is <span class="tex-font-style-bf">divisible by $3$</span>) — the number of characters in $s$.</p><p>The second line contains the string $s$ consisting of exactly $n$ characters '<span class="tex-font-style-tt">0</span>', '<span class="tex-font-style-tt">1</span>' and '<span class="tex-font-style-tt">2</span>'.</p></div><div class="output-specification"><p>Print one string — the lexicographically (alphabetically) smallest <span class="tex-font-style-it">balanced</span> ternary string which can be obtained from the given one with <span class="tex-font-style-bf">minimum</span> number of replacements.</p><p>Because $n$ is <span class="tex-font-style-bf">divisible by $3$</span> it is obvious that the answer exists. And it is obvious that there is only one possible answer.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($3 \le n \le 3 \cdot 10^5$, $n$ is <span class="tex-font-style-bf">divisible by $3$</span>) — the number of characters in $s$.</p><p>The second line contains the string $s$ consisting of exactly $n$ characters '<span class="tex-font-style-tt">0</span>', '<span class="tex-font-style-tt">1</span>' and '<span class="tex-font-style-tt">2</span>'.</p>

## Output

<p>Print one string — the lexicographically (alphabetically) smallest <span class="tex-font-style-it">balanced</span> ternary string which can be obtained from the given one with <span class="tex-font-style-bf">minimum</span> number of replacements.</p><p>Because $n$ is <span class="tex-font-style-bf">divisible by $3$</span> it is obvious that the answer exists. And it is obvious that there is only one possible answer.</p>





```input1
3
121
```




```input2
6
000000
```




```input3
6
211200
```




```input4
6
120110
```




```output1
021
```




```output2
001122
```




```output3
211200
```




```output4
120120
```


