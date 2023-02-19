## Description

<div><p>You are given a bracket sequence consisting of $n$ characters '<span class="tex-font-style-tt">(</span>' and/or <span class="tex-font-style-tt">)</span>'. You perform several operations with it.</p><p>During one operation, you choose the <span class="tex-font-style-bf">shortest</span> prefix of this string (some amount of first characters of the string) that is <span class="tex-font-style-bf">good</span> and remove it from the string.</p><p>The prefix is considered <span class="tex-font-style-bf">good</span> if one of the following two conditions is satisfied:</p><ul> <li> this prefix is a regular bracket sequence; </li><li> this prefix is a palindrome of length <span class="tex-font-style-bf">at least two</span>. </li></ul><p>A bracket sequence is called regular if it is possible to obtain a correct arithmetic expression by inserting characters '<span class="tex-font-style-tt">+</span>' and '<span class="tex-font-style-tt">1</span>' into this sequence. For example, sequences <span class="tex-font-style-tt">(())()</span>, <span class="tex-font-style-tt">()</span> and <span class="tex-font-style-tt">(()(()))</span> are regular, while <span class="tex-font-style-tt">)(</span>, <span class="tex-font-style-tt">(()</span> and <span class="tex-font-style-tt">(()))(</span> are not.</p><p>The bracket sequence is called palindrome if it reads the same back and forth. For example, the bracket sequences <span class="tex-font-style-tt">))</span>, <span class="tex-font-style-tt">((</span> and <span class="tex-font-style-tt">)(()</span> are palindromes, while bracket sequences <span class="tex-font-style-tt">()</span>, <span class="tex-font-style-tt">)(</span> and <span class="tex-font-style-tt">))(</span> are not palindromes.</p><p>You stop performing the operations when it's not possible to find a <span class="tex-font-style-bf">good</span> prefix. Your task is to find the number of operations you will perform on the given string and the number of remaining characters in the string.</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases. The next $2t$ lines describe test cases.</p><p>The first line of the test case contains one integer $n$ ($1 \le n \le 5 \cdot 10^5$) — the length of the bracket sequence.</p><p>The second line of the test case contains $n$ characters '<span class="tex-font-style-tt">(</span>' and/or '<span class="tex-font-style-tt">)</span>' — the bracket sequence itself.</p><p>It is guaranteed that the sum of $n$ over all test cases do not exceed $5 \cdot 10^5$ ($\sum n \le 5 \cdot 10^5$).</p></div><div class="output-specification"><p>For each test case, print two integers $c$ and $r$ — the number of operations you will perform on the given bracket sequence and the number of characters that remain in the string after performing all operations.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases. The next $2t$ lines describe test cases.</p><p>The first line of the test case contains one integer $n$ ($1 \le n \le 5 \cdot 10^5$) — the length of the bracket sequence.</p><p>The second line of the test case contains $n$ characters '<span class="tex-font-style-tt">(</span>' and/or '<span class="tex-font-style-tt">)</span>' — the bracket sequence itself.</p><p>It is guaranteed that the sum of $n$ over all test cases do not exceed $5 \cdot 10^5$ ($\sum n \le 5 \cdot 10^5$).</p>

## Output

<p>For each test case, print two integers $c$ and $r$ — the number of operations you will perform on the given bracket sequence and the number of characters that remain in the string after performing all operations.</p>





```input1
5
2
()
3
())
4
((((
5
)((()
6
)((()(
```




```output1
1 0
1 1
2 0
1 0
1 1
```


