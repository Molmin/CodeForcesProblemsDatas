## Description

<div><p>Erelong Leha was bored by calculating of the greatest common divisor of two factorials. Therefore he decided to solve some crosswords. It's well known that it is a very interesting occupation though it can be very difficult from time to time. In the course of solving one of the crosswords, Leha had to solve a simple task. You are able to do it too, aren't you?</p><p>Leha has two strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>. The hacker wants to change the string <span class="tex-span"><i>s</i></span> at such way, that it can be found in <span class="tex-span"><i>t</i></span> as a substring. All the changes should be the following: Leha chooses one position in the string <span class="tex-span"><i>s</i></span> and replaces the symbol in this position with the question mark "<span class="tex-font-style-tt">?</span>". The hacker is sure that the question mark in comparison can play the role of an arbitrary symbol. For example, if he gets string <span class="tex-span"><i>s</i></span>="<span class="tex-font-style-tt">ab?b</span>" as a result, it will appear in <span class="tex-span"><i>t</i></span>="<span class="tex-font-style-tt">aabrbb</span>" as a substring.</p><p>Guaranteed that the length of the string <span class="tex-span"><i>s</i></span> doesn't exceed the length of the string <span class="tex-span"><i>t</i></span>. Help the hacker to replace in <span class="tex-span"><i>s</i></span> as few symbols as possible so that the result of the replacements can be found in <span class="tex-span"><i>t</i></span> as a substring. The symbol "<span class="tex-font-style-tt">?</span>" should be considered equal to any other symbol.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ <i>m</i> ≤ 1000</span>) — the length of the string <span class="tex-span"><i>s</i></span> and the length of the string <span class="tex-span"><i>t</i></span> correspondingly.</p><p>The second line contains <span class="tex-span"><i>n</i></span> lowercase English letters — string <span class="tex-span"><i>s</i></span>.</p><p>The third line contains <span class="tex-span"><i>m</i></span> lowercase English letters — string <span class="tex-span"><i>t</i></span>.</p></div><div class="output-specification"><p>In the first line print single integer <span class="tex-span"><i>k</i></span> — the minimal number of symbols that need to be replaced.</p><p>In the second line print <span class="tex-span"><i>k</i></span> <span class="tex-font-style-bf">distinct</span> integers denoting the positions of symbols in the string <span class="tex-span"><i>s</i></span> which need to be replaced. Print the positions in any order. If there are several solutions print any of them. The numbering of the positions begins from one.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ <i>m</i> ≤ 1000</span>) — the length of the string <span class="tex-span"><i>s</i></span> and the length of the string <span class="tex-span"><i>t</i></span> correspondingly.</p><p>The second line contains <span class="tex-span"><i>n</i></span> lowercase English letters — string <span class="tex-span"><i>s</i></span>.</p><p>The third line contains <span class="tex-span"><i>m</i></span> lowercase English letters — string <span class="tex-span"><i>t</i></span>.</p>

## Output

<p>In the first line print single integer <span class="tex-span"><i>k</i></span> — the minimal number of symbols that need to be replaced.</p><p>In the second line print <span class="tex-span"><i>k</i></span> <span class="tex-font-style-bf">distinct</span> integers denoting the positions of symbols in the string <span class="tex-span"><i>s</i></span> which need to be replaced. Print the positions in any order. If there are several solutions print any of them. The numbering of the positions begins from one.</p>





```input1
3 5
abc
xaybz

```




```input2
4 10
abcd
ebceabazcd

```




```output1
2
2 3 

```




```output2
1
2 

```


