## Description

<div><p>ZS the Coder loves to read the dictionary. He thinks that a word is <span class="tex-font-style-it">nice</span> if there exists a <span class="tex-font-style-bf">substring</span> (contiguous segment of letters) of it of length <span class="tex-span">26</span> where each letter of English alphabet appears exactly once. In particular, if the string has length strictly less than <span class="tex-span">26</span>, no such substring exists and thus it is not nice.</p><p>Now, ZS the Coder tells you a word, where some of its letters are missing as he forgot them. He wants to determine if it is possible to fill in the missing letters so that the resulting word is nice. If it is possible, he needs you to find an example of such a word as well. Can you help him?</p></div><div class="input-specification"><p>The first and only line of the input contains a single string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 50 000</span>), the word that ZS the Coder remembers. Each character of the string is the uppercase letter of English alphabet ('A'-'Z') or is a question mark ('?'), where the question marks denotes the letters that ZS the Coder can't remember.</p></div><div class="output-specification"><p>If there is no way to replace all the question marks with <span class="tex-font-style-bf">uppercase letters</span> such that the resulting word is nice, then print <span class="tex-span"> - 1</span> in the only line.</p><p>Otherwise, print a string which denotes a possible nice word that ZS the Coder learned. This string should match the string from the input, except for the question marks replaced with uppercase English letters.</p><p>If there are multiple solutions, you may print any of them.</p></div>

## Input

<p>The first and only line of the input contains a single string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 50 000</span>), the word that ZS the Coder remembers. Each character of the string is the uppercase letter of English alphabet ('A'-'Z') or is a question mark ('?'), where the question marks denotes the letters that ZS the Coder can't remember.</p>

## Output

<p>If there is no way to replace all the question marks with <span class="tex-font-style-bf">uppercase letters</span> such that the resulting word is nice, then print <span class="tex-span"> - 1</span> in the only line.</p><p>Otherwise, print a string which denotes a possible nice word that ZS the Coder learned. This string should match the string from the input, except for the question marks replaced with uppercase English letters.</p><p>If there are multiple solutions, you may print any of them.</p>





```input1
ABC??FGHIJK???OPQR?TUVWXY?

```




```input2
WELCOMETOCODEFORCESROUNDTHREEHUNDREDANDSEVENTYTWO

```




```input3
??????????????????????????

```




```input4
AABCDEFGHIJKLMNOPQRSTUVW??M

```




```output1
ABCDEFGHIJKLMNOPQRZTUVWXYS
```




```output2
-1
```




```output3
MNBVCXZLKJHGFDSAQPWOEIRUYT
```




```output4
-1
```



## Note

<p>In the first sample case, <span class="tex-font-style-tt">ABCDEFGHIJKLMNOPQRZTUVWXYS</span> is a valid answer beacuse it contains a substring of length <span class="tex-span">26</span> (the whole string in this case) which contains all the letters of the English alphabet exactly once. Note that there are many possible solutions, such as <span class="tex-font-style-tt">ABCDEFGHIJKLMNOPQRSTUVWXYZ</span> or <span class="tex-font-style-tt">ABCEDFGHIJKLMNOPQRZTUVWXYS</span>.</p><p>In the second sample case, there are no missing letters. In addition, the given string does not have a substring of length <span class="tex-span">26</span> that contains all the letters of the alphabet, so the answer is <span class="tex-span"> - 1</span>.</p><p>In the third sample case, any string of length <span class="tex-span">26</span> that contains all letters of the English alphabet fits as an answer.</p>
