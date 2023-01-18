## Description

<div><p>String <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span> is called <span class="tex-span"><i>k</i></span>-palindrome, if it is a palindrome itself, and its prefix and suffix of length <img align="middle" class="tex-formula" src="file://JxTNG5fT.png" style="max-width: 100.0%;max-height: 100.0%;"> are <span class="tex-span">(<i>k</i> - 1)</span>-palindromes. By definition, any string (even empty) is 0-palindrome.</p><p>Let's call the palindrome degree of string <span class="tex-span"><i>s</i></span> such a maximum number <span class="tex-span"><i>k</i></span>, for which <span class="tex-span"><i>s</i></span> is <span class="tex-span"><i>k</i></span>-palindrome. For example, "<span class="tex-font-style-tt">abaaba</span>" has degree equals to <span class="tex-span">3</span>.</p><p>You are given a string. Your task is to find the sum of the palindrome degrees of all its prefixes.</p></div><div class="input-specification"><p>The first line of the input data contains a non-empty string, consisting of Latin letters and digits. The length of the string does not exceed <span class="tex-span">5·10<sup class="upper-index">6</sup></span>. The string is case-sensitive.</p></div><div class="output-specification"><p>Output the only number — the sum of the polindrome degrees of all the string's prefixes.</p></div>

## Input

<p>The first line of the input data contains a non-empty string, consisting of Latin letters and digits. The length of the string does not exceed <span class="tex-span">5·10<sup class="upper-index">6</sup></span>. The string is case-sensitive.</p>

## Output

<p>Output the only number — the sum of the polindrome degrees of all the string's prefixes.</p>





```input1
a2A

```




```input2
abacaba

```




```output1
1
```




```output2
6
```


