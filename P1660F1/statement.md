## Description

<div><p><span class="tex-font-style-bf">This is the easy version of Problem F. The only difference between the easy version and the hard version is the constraints.</span></p><p>We will call a non-empty string <span class="tex-font-style-bf">balanced</span> if it contains the same number of plus and minus signs. For example: strings "<span class="tex-font-style-tt">+-</span><span class="tex-font-style-tt">-+</span>" and "<span class="tex-font-style-tt">++-+-</span><span class="tex-font-style-tt">-</span>" are balanced, and strings "<span class="tex-font-style-tt">+-</span><span class="tex-font-style-tt">-</span>", "<span class="tex-font-style-tt">-</span><span class="tex-font-style-tt">-</span>" and "" are not balanced.</p><p>We will call a string <span class="tex-font-style-bf">promising</span> if the string can be made balanced by several (possibly zero) uses of the following operation:</p><ul> <li> replace two <span class="tex-font-style-bf">adjacent</span> minus signs with one plus sign. </li></ul><p>In particular, every balanced string is promising. However, the converse is not true: not every promising string is balanced.</p><p>For example, the string "<span class="tex-font-style-tt">-+-</span><span class="tex-font-style-tt">-</span><span class="tex-font-style-tt">-</span>" is promising, because you can replace two adjacent minuses with plus and get a balanced string "<span class="tex-font-style-tt">-++-</span>", or get another balanced string "<span class="tex-font-style-tt">-+-+</span>".</p><p>How many non-empty substrings of the given string $s$ are promising? Each non-empty promising substring must be counted in the answer as many times as it occurs in string $s$.</p><p>Recall that a substring is a sequence of consecutive characters of the string. For example, for string "<span class="tex-font-style-tt">+-+</span>" its substring are: "<span class="tex-font-style-tt">+-</span>", "<span class="tex-font-style-tt">-+</span>", "<span class="tex-font-style-tt">+</span>", "<span class="tex-font-style-tt">+-+</span>" (the string is a substring of itself) and some others. But the following strings are not its substring: "<span class="tex-font-style-tt">-</span><span class="tex-font-style-tt">-</span>", "<span class="tex-font-style-tt">+</span><span class="tex-font-style-tt">+</span>", "<span class="tex-font-style-tt">-</span><span class="tex-font-style-tt">++</span>".</p></div><div class="input-specification"><p>The first line of the input contains an integer $t$ ($1 \le t \le 500$)&nbsp;—the number of test cases in the test.</p><p>Then the descriptions of test cases follow.</p><p>Each test case of input data consists of two lines. The first line consists of the number $n$ ($1 \le n \le 3000$): the length of $s$.</p><p>The second line of the test case contains the string $s$ of length $n$, consisting only of characters "<span class="tex-font-style-tt">+</span>" and "<span class="tex-font-style-tt">-</span>".</p><p>It is guaranteed that the sum of values $n$ over all test cases does not exceed $3000$.</p></div><div class="output-specification"><p>For each test case, print a single number: the number of the promising non-empty substrings of string $s$. Each non-empty promising substring must be counted in the answer as many times as it occurs in string $s$.</p></div>

## Input

<p>The first line of the input contains an integer $t$ ($1 \le t \le 500$)&nbsp;—the number of test cases in the test.</p><p>Then the descriptions of test cases follow.</p><p>Each test case of input data consists of two lines. The first line consists of the number $n$ ($1 \le n \le 3000$): the length of $s$.</p><p>The second line of the test case contains the string $s$ of length $n$, consisting only of characters "<span class="tex-font-style-tt">+</span>" and "<span class="tex-font-style-tt">-</span>".</p><p>It is guaranteed that the sum of values $n$ over all test cases does not exceed $3000$.</p>

## Output

<p>For each test case, print a single number: the number of the promising non-empty substrings of string $s$. Each non-empty promising substring must be counted in the answer as many times as it occurs in string $s$.</p>





```input1
5
3
+-+
5
-+---
4
----
7
--+---+
6
+++---
```




```output1
2
4
2
7
4
```



## Note

<p>The following are the promising substrings for the first three test cases in the example:</p><ol> <li> $s[1 \dots 2]$="<span class="tex-font-style-tt">+</span><span class="tex-font-style-tt">-</span>", $s[2 \dots 3]$="<span class="tex-font-style-tt">-</span><span class="tex-font-style-tt">+</span>"; </li><li> $s[1 \dots 2]$="<span class="tex-font-style-tt">-</span><span class="tex-font-style-tt">+</span>", $s[2 \dots 3]$="<span class="tex-font-style-tt">+</span><span class="tex-font-style-tt">-</span>", $s[1 \dots 5]$="<span class="tex-font-style-tt">-</span><span class="tex-font-style-tt">+</span><span class="tex-font-style-tt">-</span><span class="tex-font-style-tt">-</span><span class="tex-font-style-tt">-</span>", $s[3 \dots 5]$="<span class="tex-font-style-tt">-</span><span class="tex-font-style-tt">-</span><span class="tex-font-style-tt">-</span>"; </li><li> $s[1 \dots 3]$="<span class="tex-font-style-tt">-</span><span class="tex-font-style-tt">-</span><span class="tex-font-style-tt">-</span>", $s[2 \dots 4]$="<span class="tex-font-style-tt">-</span><span class="tex-font-style-tt">-</span><span class="tex-font-style-tt">-</span>". </li></ol>
