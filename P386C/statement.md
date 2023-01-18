## Description

<div><p><span class="tex-font-style-it">String diversity</span> is the number of symbols that occur in the string at least once. Diversity of <span class="tex-span"><i>s</i></span> will be denoted by <span class="tex-span"><i>d</i>(<i>s</i>)</span>. For example , <span class="tex-span"><i>d</i></span>("<span class="tex-font-style-tt">aaa</span>")=1, <span class="tex-span"><i>d</i></span>("<span class="tex-font-style-tt">abacaba</span>")=3.</p><p>Given a string <span class="tex-span"><i>s</i></span>, consisting of lowercase Latin letters. Consider all its substrings. Obviously, any substring diversity is a number from 1 to <span class="tex-span"><i>d</i>(<i>s</i>)</span>. Find statistics about substrings diversity: for each <span class="tex-span"><i>k</i></span> from 1 to <span class="tex-span"><i>d</i>(<i>s</i>)</span>, find how many substrings of <span class="tex-span"><i>s</i></span> has a diversity of exactly <span class="tex-span"><i>k</i></span>.</p></div><div class="input-specification"><p>The input consists of a single line containing <span class="tex-span"><i>s</i></span>. It contains only lowercase Latin letters, the length of <span class="tex-span"><i>s</i></span> is from 1 to <span class="tex-span">3·10<sup class="upper-index">5</sup></span>.</p></div><div class="output-specification"><p>Print to the first line the value <span class="tex-span"><i>d</i>(<i>s</i>)</span>. Print sequence <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>d</i>(<i>s</i>)</sub></span> to the following lines, where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is the number of substrings of <span class="tex-span"><i>s</i></span> having diversity of exactly <span class="tex-span"><i>i</i></span>.</p></div>

## Input

<p>The input consists of a single line containing <span class="tex-span"><i>s</i></span>. It contains only lowercase Latin letters, the length of <span class="tex-span"><i>s</i></span> is from 1 to <span class="tex-span">3·10<sup class="upper-index">5</sup></span>.</p>

## Output

<p>Print to the first line the value <span class="tex-span"><i>d</i>(<i>s</i>)</span>. Print sequence <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>d</i>(<i>s</i>)</sub></span> to the following lines, where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is the number of substrings of <span class="tex-span"><i>s</i></span> having diversity of exactly <span class="tex-span"><i>i</i></span>.</p>





```input1
abca

```




```input2
aabacaabbad

```




```output1
3
4
3
3

```




```output2
4
14
19
28
5

```



## Note

<p>Consider the first example.</p><p>We denote by <span class="tex-span"><i>s</i>(<i>i</i>, <i>j</i>)</span> a substring of "<span class="tex-font-style-tt">abca</span>" with the indices in the segment <span class="tex-span">[<i>i</i>, <i>j</i>]</span>.</p><ul> <li> <span class="tex-span"><i>s</i>(1, 1) = </span> "<span class="tex-font-style-tt">a</span>", <span class="tex-span"><i>d</i>(</span>"<span class="tex-font-style-tt">a</span>"<span class="tex-span">) = 1</span> </li><li> <span class="tex-span"><i>s</i>(2, 2) = </span> "<span class="tex-font-style-tt">b</span>", <span class="tex-span"><i>d</i>(</span>"<span class="tex-font-style-tt">b</span>"<span class="tex-span">) = 1</span> </li><li> <span class="tex-span"><i>s</i>(3, 3) = </span> "<span class="tex-font-style-tt">c</span>", <span class="tex-span"><i>d</i>(</span>"<span class="tex-font-style-tt">c</span>"<span class="tex-span">) = 1</span> </li><li> <span class="tex-span"><i>s</i>(4, 4) = </span> "<span class="tex-font-style-tt">a</span>", <span class="tex-span"><i>d</i>(</span>"<span class="tex-font-style-tt">a</span>"<span class="tex-span">) = 1</span> </li><li> <span class="tex-span"><i>s</i>(1, 2) = </span> "<span class="tex-font-style-tt">ab</span>", <span class="tex-span"><i>d</i>(</span>"<span class="tex-font-style-tt">ab</span>"<span class="tex-span">) = 2</span> </li><li> <span class="tex-span"><i>s</i>(2, 3) = </span> "<span class="tex-font-style-tt">bc</span>", <span class="tex-span"><i>d</i>(</span>"<span class="tex-font-style-tt">bc</span>"<span class="tex-span">) = 2</span> </li><li> <span class="tex-span"><i>s</i>(3, 4) = </span> "<span class="tex-font-style-tt">ca</span>", <span class="tex-span"><i>d</i>(</span>"<span class="tex-font-style-tt">ca</span>"<span class="tex-span">) = 2</span> </li><li> <span class="tex-span"><i>s</i>(1, 3) = </span> "<span class="tex-font-style-tt">abc</span>", <span class="tex-span"><i>d</i>(</span>"<span class="tex-font-style-tt">abc</span>"<span class="tex-span">) = 3</span> </li><li> <span class="tex-span"><i>s</i>(2, 4) = </span> "<span class="tex-font-style-tt">bca</span>", <span class="tex-span"><i>d</i>(</span>"<span class="tex-font-style-tt">bca</span>"<span class="tex-span">) = 3</span> </li><li> <span class="tex-span"><i>s</i>(1, 4) = </span> "<span class="tex-font-style-tt">abca</span>", <span class="tex-span"><i>d</i>(</span>"<span class="tex-font-style-tt">abca</span>"<span class="tex-span">) = 3</span> </li></ul><p>Total number of substring with diversity 1 is 4, with diversity 2 equals 3, 3 diversity is 3.</p>
