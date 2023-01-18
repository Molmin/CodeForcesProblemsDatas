## Description

<div><p>Vasya is preparing a contest, and now he has written a statement for an easy problem. The statement is a string of length $n$ consisting of lowercase Latin latters. Vasya thinks that the statement can be considered hard if it contains a subsequence <span class="tex-font-style-tt">hard</span>; otherwise the statement is easy. For example, <span class="tex-font-style-tt">hard</span>, <span class="tex-font-style-tt">hzazrzd</span>, <span class="tex-font-style-tt">haaaaard</span> can be considered hard statements, while <span class="tex-font-style-tt">har</span>, <span class="tex-font-style-tt">hart</span> and <span class="tex-font-style-tt">drah</span> are easy statements. </p><p>Vasya doesn't want the statement to be hard. He may remove some characters from the statement in order to make it easy. But, of course, some parts of the statement can be crucial to understanding. Initially the <span class="tex-font-style-it">ambiguity</span> of the statement is $0$, and removing $i$-th character increases the <span class="tex-font-style-it">ambiguity</span> by $a_i$ (the index of each character is considered as it was in the original statement, so, for example, if you delete character <span class="tex-font-style-tt">r</span> from <span class="tex-font-style-tt">hard</span>, and then character <span class="tex-font-style-tt">d</span>, the index of <span class="tex-font-style-tt">d</span> is still $4$ even though you delete it from the string <span class="tex-font-style-tt">had</span>).</p><p>Vasya wants to calculate the minimum <span class="tex-font-style-it">ambiguity</span> of the statement, if he removes some characters (possibly zero) so that the statement is easy. Help him to do it!</p><p>Recall that subsequence is a sequence that can be derived from another sequence by deleting some elements without changing the order of the remaining elements.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 10^5$) — the length of the statement.</p><p>The second line contains one string $s$ of length $n$, consisting of lowercase Latin letters — the statement written by Vasya.</p><p>The third line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 998244353$).</p></div><div class="output-specification"><p>Print minimum possible <span class="tex-font-style-it">ambiguity</span> of the statement after Vasya deletes some (possibly zero) characters so the resulting statement is easy.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 10^5$) — the length of the statement.</p><p>The second line contains one string $s$ of length $n$, consisting of lowercase Latin letters — the statement written by Vasya.</p><p>The third line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 998244353$).</p>

## Output

<p>Print minimum possible <span class="tex-font-style-it">ambiguity</span> of the statement after Vasya deletes some (possibly zero) characters so the resulting statement is easy.</p>





```input1
6
hhardh
3 2 9 11 7 1
```




```input2
8
hhzarwde
3 2 6 9 4 8 7 1
```




```input3
6
hhaarr
1 2 3 4 5 6
```




```output1
5
```




```output2
4
```




```output3
0
```



## Note

<p>In the first example, first two characters are removed so the result is <span class="tex-font-style-tt">ardh</span>.</p><p>In the second example, $5$-th character is removed so the result is <span class="tex-font-style-tt">hhzawde</span>.</p><p>In the third example there's no need to remove anything.</p>
