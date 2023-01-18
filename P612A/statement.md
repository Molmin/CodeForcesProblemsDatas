## Description

<div><p>You are given the string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span> and the numbers <span class="tex-span"><i>p</i>, <i>q</i></span>. Split the string <span class="tex-span"><i>s</i></span> to pieces of length <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span>.</p><p>For example, the string "<span class="tex-font-style-tt">Hello</span>" for <span class="tex-span"><i>p</i> = 2</span>, <span class="tex-span"><i>q</i> = 3</span> can be split to the two strings "<span class="tex-font-style-tt">Hel</span>" and "<span class="tex-font-style-tt">lo</span>" or to the two strings "<span class="tex-font-style-tt">He</span>" and "<span class="tex-font-style-tt">llo</span>".</p><p>Note it is allowed to split the string <span class="tex-span"><i>s</i></span> to the strings only of length <span class="tex-span"><i>p</i></span> or to the strings only of length <span class="tex-span"><i>q</i></span> (see the second sample test).</p></div><div class="input-specification"><p>The first line contains three positive integers <span class="tex-span"><i>n</i>, <i>p</i>, <i>q</i></span> (<span class="tex-span">1 ≤ <i>p</i>, <i>q</i> ≤ <i>n</i> ≤ 100</span>).</p><p>The second line contains the string <span class="tex-span"><i>s</i></span> consists of lowercase and uppercase latin letters and digits.</p></div><div class="output-specification"><p>If it's impossible to split the string <span class="tex-span"><i>s</i></span> to the strings of length <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span> print the only number "<span class="tex-font-style-tt">-1</span>".</p><p>Otherwise in the first line print integer <span class="tex-span"><i>k</i></span> — the number of strings in partition of <span class="tex-span"><i>s</i></span>.</p><p>Each of the next <span class="tex-span"><i>k</i></span> lines should contain the strings in partition. Each string should be of the length <span class="tex-span"><i>p</i></span> or <span class="tex-span"><i>q</i></span>. The string should be in order of their appearing in string <span class="tex-span"><i>s</i></span> — from left to right.</p><p>If there are several solutions print any of them.</p></div>

## Input

<p>The first line contains three positive integers <span class="tex-span"><i>n</i>, <i>p</i>, <i>q</i></span> (<span class="tex-span">1 ≤ <i>p</i>, <i>q</i> ≤ <i>n</i> ≤ 100</span>).</p><p>The second line contains the string <span class="tex-span"><i>s</i></span> consists of lowercase and uppercase latin letters and digits.</p>

## Output

<p>If it's impossible to split the string <span class="tex-span"><i>s</i></span> to the strings of length <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span> print the only number "<span class="tex-font-style-tt">-1</span>".</p><p>Otherwise in the first line print integer <span class="tex-span"><i>k</i></span> — the number of strings in partition of <span class="tex-span"><i>s</i></span>.</p><p>Each of the next <span class="tex-span"><i>k</i></span> lines should contain the strings in partition. Each string should be of the length <span class="tex-span"><i>p</i></span> or <span class="tex-span"><i>q</i></span>. The string should be in order of their appearing in string <span class="tex-span"><i>s</i></span> — from left to right.</p><p>If there are several solutions print any of them.</p>





```input1
5 2 3
Hello

```




```input2
10 9 5
Codeforces

```




```input3
6 4 5
Privet

```




```input4
8 1 1
abacabac

```




```output1
2
He
llo

```




```output2
2
Codef
orces

```




```output3
-1

```




```output4
8
a
b
a
c
a
b
a
c

```


