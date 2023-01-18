## Description

<div><p>A string is a palindrome if it reads the same from the left to the right and from the right to the left. For example, the strings "<span class="tex-font-style-tt">kek</span>", "<span class="tex-font-style-tt">abacaba</span>", "<span class="tex-font-style-tt">r</span>" and "<span class="tex-font-style-tt">papicipap</span>" are palindromes, while the strings "<span class="tex-font-style-tt">abb</span>" and "<span class="tex-font-style-tt">iq</span>" are not.</p><p>A substring $s[l \ldots r]$ ($1 \leq l \leq r \leq |s|$) of a string $s = s_{1}s_{2} \ldots s_{|s|}$ is the string $s_{l}s_{l + 1} \ldots s_{r}$.</p><p>Anna does not like palindromes, so she makes her friends call her Ann. She also changes all the words she reads in a similar way. Namely, each word $s$ is changed into its longest substring that is not a palindrome. If all the substrings of $s$ are palindromes, she skips the word at all.</p><p>Some time ago Ann read the word $s$. What is the word she changed it into?</p></div><div class="input-specification"><p>The first line contains a non-empty string $s$ with length at most $50$ characters, containing lowercase English letters only.</p></div><div class="output-specification"><p>If there is such a substring in $s$ that is not a palindrome, print the maximum length of such a substring. Otherwise print $0$.</p><p>Note that there can be multiple longest substrings that are not palindromes, but their length is unique.</p></div>

## Input

<p>The first line contains a non-empty string $s$ with length at most $50$ characters, containing lowercase English letters only.</p>

## Output

<p>If there is such a substring in $s$ that is not a palindrome, print the maximum length of such a substring. Otherwise print $0$.</p><p>Note that there can be multiple longest substrings that are not palindromes, but their length is unique.</p>





```input1
mew

```




```input2
wuffuw

```




```input3
qqqqqqqq

```




```output1
3

```




```output2
5

```




```output3
0

```



## Note

<p>"<span class="tex-font-style-tt">mew</span>" is not a palindrome, so the longest substring of it that is not a palindrome, is the string "<span class="tex-font-style-tt">mew</span>" itself. Thus, the answer for the first example is $3$.</p><p>The string "<span class="tex-font-style-tt">uffuw</span>" is one of the longest non-palindrome substrings (of length $5$) of the string "<span class="tex-font-style-tt">wuffuw</span>", so the answer for the second example is $5$.</p><p>All substrings of the string "<span class="tex-font-style-tt">qqqqqqqq</span>" consist of equal characters so they are palindromes. This way, there are no non-palindrome substrings. Thus, the answer for the third example is $0$.</p>
