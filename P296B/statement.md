## Description

<div><p>Yaroslav thinks that two strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>w</i></span>, consisting of digits and having length <span class="tex-span"><i>n</i></span> are non-comparable if there are two numbers, <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> <span class="tex-span">(1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i>)</span>, such that <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> &gt; <i>w</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index"><i>j</i></sub> &lt; <i>w</i><sub class="lower-index"><i>j</i></sub></span>. Here sign <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> represents the <span class="tex-span"><i>i</i></span>-th digit of string <span class="tex-span"><i>s</i></span>, similarly, <span class="tex-span"><i>w</i><sub class="lower-index"><i>j</i></sub></span> represents the <span class="tex-span"><i>j</i></span>-th digit of string <span class="tex-span"><i>w</i></span>.</p><p>A string's template is a string that consists of digits and question marks ("<span class="tex-font-style-tt">?</span>").</p><p>Yaroslav has two string templates, each of them has length <span class="tex-span"><i>n</i></span>. Yaroslav wants to count the number of ways to replace all question marks by some integers in both templates, so as to make the resulting strings incomparable. Note that the obtained strings can contain leading zeroes and that distinct question marks can be replaced by distinct or the same integers.</p><p>Help Yaroslav, calculate the remainder after dividing the described number of ways by <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the length of both templates. The second line contains the first template — a string that consists of digits and characters "<span class="tex-font-style-tt">?</span>". The string's length equals <span class="tex-span"><i>n</i></span>. The third line contains the second template in the same format.</p></div><div class="output-specification"><p>In a single line print the remainder after dividing the answer to the problem by number <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the length of both templates. The second line contains the first template — a string that consists of digits and characters "<span class="tex-font-style-tt">?</span>". The string's length equals <span class="tex-span"><i>n</i></span>. The third line contains the second template in the same format.</p>

## Output

<p>In a single line print the remainder after dividing the answer to the problem by number <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
2
90
09

```




```input2
2
11
55

```




```input3
5
?????
?????

```




```output1
1

```




```output2
0

```




```output3
993531194

```



## Note

<p>The first test contains no question marks and both strings are incomparable, so the answer is <span class="tex-span">1</span>.</p><p>The second test has no question marks, but the given strings are comparable, so the answer is <span class="tex-span">0</span>.</p>
