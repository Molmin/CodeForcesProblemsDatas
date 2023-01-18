## Description

<div><p>You are given a string $s$ consisting only of first $20$ lowercase Latin letters ('<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>', ..., '<span class="tex-font-style-tt">t</span>').</p><p>Recall that the substring $s[l; r]$ of the string $s$ is the string $s_l s_{l + 1} \dots s_r$. For example, the substrings of "<span class="tex-font-style-tt">codeforces</span>" are "<span class="tex-font-style-tt">code</span>", "<span class="tex-font-style-tt">force</span>", "<span class="tex-font-style-tt">f</span>", "<span class="tex-font-style-tt">for</span>", but not "<span class="tex-font-style-tt">coder</span>" and "<span class="tex-font-style-tt">top</span>".</p><p>You can perform the following operation <span class="tex-font-style-bf">no more than once</span>: choose some substring $s[l; r]$ and <span class="tex-font-style-bf">reverse</span> it (i.e. the string $s_l s_{l + 1} \dots s_r$ becomes $s_r s_{r - 1} \dots s_l$).</p><p>Your goal is to maximize the length of the maximum substring of $s$ consisting of <span class="tex-font-style-bf">distinct</span> (i.e. unique) characters.</p><p>The string consists of <span class="tex-font-style-bf">distinct</span> characters if no character in this string appears more than once. For example, strings "<span class="tex-font-style-tt">abcde</span>", "<span class="tex-font-style-tt">arctg</span>" and "<span class="tex-font-style-tt">minecraft</span>" consist of distinct characters but strings "<span class="tex-font-style-tt">codeforces</span>", "<span class="tex-font-style-tt">abacaba</span>" do not consist of distinct characters.</p></div><div class="input-specification"><p>The only line of the input contains one string $s$ consisting of no more than $10^6$ characters '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>', ..., '<span class="tex-font-style-tt">t</span>' (first $20$ lowercase Latin letters).</p></div><div class="output-specification"><p>Print one integer — the maximum possible length of the maximum substring of $s$ consisting of distinct characters after reversing no more than one its substring.</p></div>

## Input

<p>The only line of the input contains one string $s$ consisting of no more than $10^6$ characters '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>', ..., '<span class="tex-font-style-tt">t</span>' (first $20$ lowercase Latin letters).</p>

## Output

<p>Print one integer — the maximum possible length of the maximum substring of $s$ consisting of distinct characters after reversing no more than one its substring.</p>





```input1
abacaba
```




```input2
abcdecdf
```




```input3
aabbcc
```




```input4
abcdeefc
```




```output1
3
```




```output2
6
```




```output3
3
```




```output4
6
```


