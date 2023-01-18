## Description

<div><p>A <span class="tex-font-style-it">tree</span> is a connected undirected graph with <span class="tex-span"><i>n</i> - 1</span> edges, where <span class="tex-span"><i>n</i></span> denotes the number of vertices. Vertices are numbered <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span>.</p><p>Limak is a little polar bear. His bear family prepares a New Year tree every year. One year ago their tree was more awesome than usually. Thus, they decided to prepare the same tree in the next year. Limak was responsible for remembering that tree.</p><p>It would be hard to remember a whole tree. Limak decided to describe it in his notebook instead. He took a pen and wrote <span class="tex-span"><i>n</i> - 1</span> lines, each with two integers&nbsp;— indices of two vertices connected by an edge.</p><p>Now, the New Year is just around the corner and Limak is asked to reconstruct that tree. Of course, there is a problem. He was a very little bear a year ago, and he didn't know digits and the alphabet, so he just replaced each digit with a question mark&nbsp;— the only character he knew. That means, for any vertex index in his notes he knows only the number of digits in it. At least he knows there were no leading zeroes.</p><p>Limak doesn't want to disappoint everyone. Please, take his notes and reconstruct a New Year tree. Find any tree matching Limak's records and print its edges in any order. It's also possible that Limak made a mistake and there is no suitable tree&nbsp;– in this case print "<span class="tex-font-style-tt">-1</span>" (without the quotes).</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of vertices.</p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains two space-separated non-empty strings, both consisting of questions marks only. No string has more characters than the number of digits in <span class="tex-span"><i>n</i></span>.</p></div><div class="output-specification"><p>If there is no tree matching Limak's records, print the only line with "<span class="tex-font-style-tt">-1</span>" (without the quotes).</p><p>Otherwise, describe any tree matching Limak's notes. Print <span class="tex-span"><i>n</i> - 1</span> lines, each with two space-separated integers&nbsp;– indices of vertices connected by an edge. You can print edges in any order.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of vertices.</p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains two space-separated non-empty strings, both consisting of questions marks only. No string has more characters than the number of digits in <span class="tex-span"><i>n</i></span>.</p>

## Output

<p>If there is no tree matching Limak's records, print the only line with "<span class="tex-font-style-tt">-1</span>" (without the quotes).</p><p>Otherwise, describe any tree matching Limak's notes. Print <span class="tex-span"><i>n</i> - 1</span> lines, each with two space-separated integers&nbsp;– indices of vertices connected by an edge. You can print edges in any order.</p>





```input1
12
? ?
? ?
? ?
? ??
?? ?
?? ??
? ??
? ?
? ?
? ?
? ?

```




```input2
12
?? ??
? ?
? ?
? ??
?? ?
?? ??
? ??
? ?
? ?
?? ??
? ?

```




```output1
3 1
1 6
9 1
2 10
1 7
8 1
1 4
1 10
5 1
10 11
12 1

```




```output2
-1

```


