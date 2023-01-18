## Description

<div><p>In his very young years the hero of our story, king Copa, decided that his private data was hidden not enough securely, what is unacceptable for the king. That's why he invented tricky and clever password (later he learned that his password is a palindrome of odd length), and coded all his data using it. </p><p>Copa is afraid to forget his password, so he decided to write it on a piece of paper. He is aware that it is insecure to keep password in such way, so he decided to cipher it the following way: he cut <span class="tex-span"><i>x</i></span> characters from the start of his password and from the end of it (<span class="tex-span"><i>x</i></span> can be <span class="tex-span">0</span>, and <span class="tex-span">2<i>x</i></span> is strictly less than the password length). He obtained 3 <span class="tex-font-style-bf"><span class="tex-font-style-underline">parts of the password</span></span>. Let's call it <span class="tex-span"><i>prefix</i></span>, <span class="tex-span"><i>middle</i></span> and <span class="tex-span"><i>suffix</i></span> correspondingly, both <span class="tex-span"><i>prefix</i></span> and <span class="tex-span"><i>suffix</i></span> having equal length and <span class="tex-span"><i>middle</i></span> always having odd length. From these parts he made a string <span class="tex-span"><i>A</i> + <i>prefix</i> + <i>B</i> + <i>middle</i> + <i>C</i> + <i>suffix</i></span>, where <span class="tex-span"><i>A</i></span>, <span class="tex-span"><i>B</i></span> and <span class="tex-span"><i>C</i></span> are some (possibly empty) strings invented by Copa, and «<span class="tex-span"> + </span>» means concatenation.</p><p>Many years have passed, and just yesterday the king Copa found the piece of paper where his ciphered password was written. The password, as well as the strings <span class="tex-span"><i>A</i></span>, <span class="tex-span"><i>B</i></span> and <span class="tex-span"><i>C</i></span>, was completely forgotten by Copa, so he asks you to find a password of maximum possible length, which could be invented, ciphered and written by Copa.</p></div><div class="input-specification"><p>The input contains single string of small Latin letters with length from <span class="tex-span">1</span> to <span class="tex-span">10<sup class="upper-index">5</sup></span> characters.</p></div><div class="output-specification"><p>The first line should contain integer <span class="tex-span"><i>k</i></span> — amount of <span class="tex-font-style-bf"><span class="tex-font-style-underline">nonempty parts of the password</span></span> in your answer (<img align="middle" class="tex-formula" src="file://6hBH8Jz8.png" style="max-width: 100.0%;max-height: 100.0%;">). In each of the following <span class="tex-span"><i>k</i></span> lines output two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> — start and length of the corresponding part of the password. Output pairs in order of increasing <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>. Separate the numbers in pairs by a single space.</p><p>Starting position <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> should be an integer from <span class="tex-span">1</span> to the length of the input string. All <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> must be positive, because you should output only non-empty parts. The middle part must have odd length.</p><p>If there are several solutions, output any. Note that your goal is to maximize the sum of <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, but not to maximize <span class="tex-span"><i>k</i></span>.</p></div>

## Input

<p>The input contains single string of small Latin letters with length from <span class="tex-span">1</span> to <span class="tex-span">10<sup class="upper-index">5</sup></span> characters.</p>

## Output

<p>The first line should contain integer <span class="tex-span"><i>k</i></span> — amount of <span class="tex-font-style-bf"><span class="tex-font-style-underline">nonempty parts of the password</span></span> in your answer (<img align="middle" class="tex-formula" src="file://6hBH8Jz8.png" style="max-width: 100.0%;max-height: 100.0%;">). In each of the following <span class="tex-span"><i>k</i></span> lines output two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> — start and length of the corresponding part of the password. Output pairs in order of increasing <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>. Separate the numbers in pairs by a single space.</p><p>Starting position <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> should be an integer from <span class="tex-span">1</span> to the length of the input string. All <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> must be positive, because you should output only non-empty parts. The middle part must have odd length.</p><p>If there are several solutions, output any. Note that your goal is to maximize the sum of <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, but not to maximize <span class="tex-span"><i>k</i></span>.</p>





```input1
abacaba

```




```input2
axbya

```




```input3
xabyczba

```




```output1
1
1 7

```




```output2
3
1 1
2 1
5 1

```




```output3
3
2 2
4 1
7 2

```


