## Description

<div><p>Let's call a string <span class="tex-font-style-it">good</span> if and only if it consists of only two types of letters&nbsp;— '<span class="tex-font-style-tt">a</span>' and '<span class="tex-font-style-tt">b</span>' and every two consecutive letters are distinct. For example "<span class="tex-font-style-tt">baba</span>" and "<span class="tex-font-style-tt">aba</span>" are good strings and "<span class="tex-font-style-tt">abb</span>" is a bad string.</p><p>You have $a$ strings "<span class="tex-font-style-tt">a</span>", $b$ strings "<span class="tex-font-style-tt">b</span>" and $c$ strings "<span class="tex-font-style-tt">ab</span>". You want to choose some subset of these strings and concatenate them in any arbitrarily order.</p><p>What is the length of the longest good string you can obtain this way?</p></div><div class="input-specification"><p>The first line contains three positive integers $a$, $b$, $c$ ($1 \leq a, b, c \leq 10^9$)&nbsp;— the number of strings "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>" and "<span class="tex-font-style-tt">ab</span>" respectively.</p></div><div class="output-specification"><p>Print a single number&nbsp;— the maximum possible length of the good string you can obtain.</p></div>

## Input

<p>The first line contains three positive integers $a$, $b$, $c$ ($1 \leq a, b, c \leq 10^9$)&nbsp;— the number of strings "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>" and "<span class="tex-font-style-tt">ab</span>" respectively.</p>

## Output

<p>Print a single number&nbsp;— the maximum possible length of the good string you can obtain.</p>





```input1
1 1 1
```




```input2
2 1 2
```




```input3
3 5 2
```




```input4
2 2 1
```




```input5
1000000000 1000000000 1000000000
```




```output1
4
```




```output2
7
```




```output3
11
```




```output4
6
```




```output5
4000000000
```



## Note

<p>In the first example the optimal string is "<span class="tex-font-style-tt">baba</span>".</p><p>In the second example the optimal string is "<span class="tex-font-style-tt">abababa</span>".</p><p>In the third example the optimal string is "<span class="tex-font-style-tt">bababababab</span>".</p><p>In the fourth example the optimal string is "<span class="tex-font-style-tt">ababab</span>".</p>
