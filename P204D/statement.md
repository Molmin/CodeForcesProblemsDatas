## Description

<div><p>The Little Elephant has found a ragged old black-and-white string <span class="tex-span"><i>s</i></span> on the attic.</p><p>The characters of string <span class="tex-span"><i>s</i></span> are numbered from the left to the right from <span class="tex-span">1</span> to <span class="tex-span">|<i>s</i>|</span>, where <span class="tex-span">|<i>s</i>|</span> is the length of the string. Let's denote the <span class="tex-span"><i>i</i></span>-th character of string <span class="tex-span"><i>s</i></span> as <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>. As the string is black-and-white, each character of the string is either letter "<span class="tex-font-style-tt">B</span>", or letter "<span class="tex-font-style-tt">W</span>". Unfortunately, the string is very old and some characters are damaged. The damaged positions are denoted as "<span class="tex-font-style-tt">X</span>".</p><p>The Little Elephant in determined to restore the string and hang it on the wall. For that he needs to replace each character "<span class="tex-font-style-tt">X</span>" by a "<span class="tex-font-style-tt">B</span>" or a "<span class="tex-font-style-tt">W</span>". The string must look good on the wall, so it must be <span class="tex-font-style-underline">beautiful</span>. The Little Elephant considers a string beautiful if it has two non-intersecting substrings of a given length <span class="tex-span"><i>k</i></span>, such that the left one fully consists of characters "<span class="tex-font-style-tt">B</span>", and the right one fully consists of characters "<span class="tex-font-style-tt">W</span>". More formally, there are four integers <span class="tex-span"><i>a</i>, <i>b</i>, <i>c</i>, <i>d</i></span> <span class="tex-span">(1 ≤ <i>a</i> ≤ <i>b</i> &lt; <i>c</i> ≤ <i>d</i> ≤ |<i>s</i>|;&nbsp;<i>b</i> - <i>a</i> + 1 = <i>d</i> - <i>c</i> + 1 = <i>k</i>)</span> such that <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> = "<span class="tex-font-style-tt">B</span>" <span class="tex-span">(<i>a</i> ≤ <i>i</i> ≤ <i>b</i>)</span> and <span class="tex-span"><i>s</i><sub class="lower-index"><i>j</i></sub></span> = "<span class="tex-font-style-tt">W</span>" <span class="tex-span">(<i>c</i> ≤ <i>j</i> ≤ <i>d</i>)</span>. </p><p>Help the Little Elephant find the number of different beautiful strings he can obtain from string <span class="tex-span"><i>s</i></span>. Two strings are considered different if there is such position, where the character in the first string differs from the corresponding character in the second string. If this string doesn't contain characters «<span class="tex-font-style-tt">X</span>» and it is already beautiful — the answer is <span class="tex-font-style-tt">1</span>.</p><p>As the answer can be rather large, print it modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>)</span>. The second line contains string <span class="tex-span"><i>s</i></span>. String <span class="tex-span"><i>s</i></span> has length <span class="tex-span"><i>n</i></span> and only consists of characters "<span class="tex-font-style-tt">W</span>", "<span class="tex-font-style-tt">B</span>" and "<span class="tex-font-style-tt">X</span>".</p></div><div class="output-specification"><p>On a single line print an integer — the answer to the problem modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>)</span>. The second line contains string <span class="tex-span"><i>s</i></span>. String <span class="tex-span"><i>s</i></span> has length <span class="tex-span"><i>n</i></span> and only consists of characters "<span class="tex-font-style-tt">W</span>", "<span class="tex-font-style-tt">B</span>" and "<span class="tex-font-style-tt">X</span>".</p>

## Output

<p>On a single line print an integer — the answer to the problem modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
3 2
XXX

```




```input2
4 2
XXXX

```




```input3
10 2
XXBXXWXXXX

```




```output1
0

```




```output2
1

```




```output3
166

```


