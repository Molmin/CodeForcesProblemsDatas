## Description

<div><p>After Fox Ciel got off a bus, she found that the bus she was on was a wrong bus and she lost her way in a strange town. However, she fortunately met her friend Beaver Taro and asked which way to go to her castle. Taro's response to her was a string <span class="tex-span"><i>s</i></span>, and she tried to remember the string <span class="tex-span"><i>s</i></span> correctly.</p><p>However, Ciel feels <span class="tex-span"><i>n</i></span> strings <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ... , <i>b</i><sub class="lower-index"><i>n</i></sub></span> are really boring, and unfortunately she dislikes to remember a string that contains a boring substring. To make the thing worse, what she can remember is only the contiguous substring of <span class="tex-span"><i>s</i></span>.</p><p>Determine the longest contiguous substring of <span class="tex-span"><i>s</i></span> that does not contain any boring string, so that she can remember the longest part of Taro's response.</p></div><div class="input-specification"><p>In the first line there is a string <span class="tex-span"><i>s</i></span>. The length of <span class="tex-span"><i>s</i></span> will be between <span class="tex-span">1</span> and <span class="tex-span">10<sup class="upper-index">5</sup></span>, inclusive.</p><p>In the second line there is a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10</span>).  Next <span class="tex-span"><i>n</i></span> lines, there is a string <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>). Each length of <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> will be between <span class="tex-span">1</span> and <span class="tex-span">10</span>, inclusive.</p><p>Each character of the given strings will be either a English alphabet (both lowercase and uppercase) or a underscore (<span class="tex-font-style-tt">'_'</span>) or a digit. Assume that these strings are case-sensitive.</p></div><div class="output-specification"><p>Output in the first line two space-separated integers <span class="tex-span"><i>len</i></span> and <span class="tex-span"><i>pos</i></span>: the length of the longest contiguous substring of <span class="tex-span"><i>s</i></span> that does not contain any <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, and the first position of the substring (0-indexed). The position <span class="tex-span"><i>pos</i></span> must be between <span class="tex-span">0</span> and <span class="tex-span">|<i>s</i>| - <i>len</i></span> inclusive, where <span class="tex-span">|<i>s</i>|</span> is the length of string <span class="tex-span"><i>s</i></span>.</p><p>If there are several solutions, output any.</p></div>

## Input

<p>In the first line there is a string <span class="tex-span"><i>s</i></span>. The length of <span class="tex-span"><i>s</i></span> will be between <span class="tex-span">1</span> and <span class="tex-span">10<sup class="upper-index">5</sup></span>, inclusive.</p><p>In the second line there is a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10</span>).  Next <span class="tex-span"><i>n</i></span> lines, there is a string <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>). Each length of <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> will be between <span class="tex-span">1</span> and <span class="tex-span">10</span>, inclusive.</p><p>Each character of the given strings will be either a English alphabet (both lowercase and uppercase) or a underscore (<span class="tex-font-style-tt">'_'</span>) or a digit. Assume that these strings are case-sensitive.</p>

## Output

<p>Output in the first line two space-separated integers <span class="tex-span"><i>len</i></span> and <span class="tex-span"><i>pos</i></span>: the length of the longest contiguous substring of <span class="tex-span"><i>s</i></span> that does not contain any <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, and the first position of the substring (0-indexed). The position <span class="tex-span"><i>pos</i></span> must be between <span class="tex-span">0</span> and <span class="tex-span">|<i>s</i>| - <i>len</i></span> inclusive, where <span class="tex-span">|<i>s</i>|</span> is the length of string <span class="tex-span"><i>s</i></span>.</p><p>If there are several solutions, output any.</p>





```input1
Go_straight_along_this_street
5
str
long
tree
biginteger
ellipse

```




```input2
IhaveNoIdea
9
I
h
a
v
e
N
o
I
d

```




```input3
unagioisii
2
ioi
unagi

```




```output1
12 4

```




```output2
0 0

```




```output3
5 5

```



## Note

<p>In the first sample, the solution is <span class="tex-font-style-tt">traight_alon</span>.</p><p>In the second sample, the solution is an empty string, so the output can be «<span class="tex-font-style-tt">0 0</span>», «<span class="tex-font-style-tt">0 1</span>», «<span class="tex-font-style-tt">0 2</span>», and so on.</p><p>In the third sample, the solution is either <span class="tex-font-style-tt">nagio</span> or <span class="tex-font-style-tt">oisii</span>.</p>
