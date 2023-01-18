## Description

<div><p>Developers often face with regular expression patterns. A pattern is usually defined as a string consisting of characters and metacharacters that sets the rules for your search. These patterns are most often used to check whether a particular string meets the certain rules.</p><p>In this task, a pattern will be a string consisting of small English letters and question marks ('<span class="tex-font-style-tt">?</span>'). The question mark in the pattern is a metacharacter that denotes an arbitrary small letter of the English alphabet. We will assume that a string matches the pattern if we can transform the string into the pattern by replacing the question marks by the appropriate characters. For example, string <span class="tex-font-style-tt">aba</span> matches patterns: <span class="tex-font-style-tt">???</span>, <span class="tex-font-style-tt">??a</span>, <span class="tex-font-style-tt">a?a</span>, <span class="tex-font-style-tt">aba</span>.</p><p>Programmers that work for the R1 company love puzzling each other (and themselves) with riddles. One of them is as follows: you are given <span class="tex-span"><i>n</i></span> patterns of the same length, you need to find a pattern that contains as few question marks as possible, and intersects with each of the given patterns. Two patterns intersect if there is a string that matches both the first and the second pattern. Can you solve this riddle?</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of patterns. Next <span class="tex-span"><i>n</i></span> lines contain the patterns.</p><p>It is guaranteed that the patterns can only consist of small English letters and symbols '<span class="tex-font-style-tt">?</span>'. All patterns are non-empty and have the same length. The total length of all the patterns does not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span> characters.</p></div><div class="output-specification"><p>In a single line print the answer to the problem — the pattern with the minimal number of signs '<span class="tex-font-style-tt">?</span>', which intersects with each of the given ones. If there are several answers, print any of them.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of patterns. Next <span class="tex-span"><i>n</i></span> lines contain the patterns.</p><p>It is guaranteed that the patterns can only consist of small English letters and symbols '<span class="tex-font-style-tt">?</span>'. All patterns are non-empty and have the same length. The total length of all the patterns does not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span> characters.</p>

## Output

<p>In a single line print the answer to the problem — the pattern with the minimal number of signs '<span class="tex-font-style-tt">?</span>', which intersects with each of the given ones. If there are several answers, print any of them.</p>





```input1
2
?ab
??b

```




```input2
2
a
b

```




```input3
1
?a?b

```




```output1
xab

```




```output2
?

```




```output3
cacb

```



## Note

<p>Consider the first example. Pattern <span class="tex-font-style-tt">xab</span> intersects with each of the given patterns. Pattern <span class="tex-font-style-tt">???</span> also intersects with each of the given patterns, but it contains more question signs, hence it is not an optimal answer. Clearly, <span class="tex-font-style-tt">xab</span> is the optimal answer, because it doesn't contain any question sign. There are a lot of other optimal answers, for example: <span class="tex-font-style-tt">aab</span>, <span class="tex-font-style-tt">bab</span>, <span class="tex-font-style-tt">cab</span>, <span class="tex-font-style-tt">dab</span> and so on.</p>
