## Description

<div><p>Misha didn't do his math homework for today's lesson once again. As a punishment, his teacher Dr. Andrew decided to give him a hard, but very useless task.</p><p>Dr. Andrew has written two strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> of lowercase English letters at the blackboard. He reminded Misha that <span class="tex-font-style-it">prefix</span> of a string is a string formed by removing several (possibly none) of its last characters, and a <span class="tex-font-style-it">concatenation</span> of two strings is a string formed by appending the second string to the right of the first string.</p><p>The teacher asked Misha to write down on the blackboard all strings that are the concatenations of some non-empty prefix of <span class="tex-span"><i>s</i></span> and some non-empty prefix of <span class="tex-span"><i>t</i></span>. When Misha did it, Dr. Andrew asked him how many distinct strings are there. Misha spent almost the entire lesson doing that and completed the task. </p><p>Now he asks you to write a program that would do this task automatically.</p></div><div class="input-specification"><p>The first line contains the string <span class="tex-span"><i>s</i></span> consisting of lowercase English letters. The second line contains the string <span class="tex-span"><i>t</i></span> consisting of lowercase English letters.</p><p>The lengths of both string do not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p></div><div class="output-specification"><p>Output a single integer&nbsp;— the number of distinct strings that are concatenations of some non-empty prefix of <span class="tex-span"><i>s</i></span> with some non-empty prefix of <span class="tex-span"><i>t</i></span>.</p></div>

## Input

<p>The first line contains the string <span class="tex-span"><i>s</i></span> consisting of lowercase English letters. The second line contains the string <span class="tex-span"><i>t</i></span> consisting of lowercase English letters.</p><p>The lengths of both string do not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p>

## Output

<p>Output a single integer&nbsp;— the number of distinct strings that are concatenations of some non-empty prefix of <span class="tex-span"><i>s</i></span> with some non-empty prefix of <span class="tex-span"><i>t</i></span>.</p>





```input1
aba
aa

```




```input2
aaaaa
aaaa

```




```output1
5

```




```output2
8

```



## Note

<p>In the first example, the string <span class="tex-span"><i>s</i></span> has three non-empty prefixes: {<span class="tex-font-style-tt">a</span>, <span class="tex-font-style-tt">ab</span>, <span class="tex-font-style-tt">aba</span>}. The string <span class="tex-span"><i>t</i></span> has two non-empty prefixes: {<span class="tex-font-style-tt">a</span>, <span class="tex-font-style-tt">aa</span>}. In total, Misha has written five distinct strings: {<span class="tex-font-style-tt">aa</span>, <span class="tex-font-style-tt">aaa</span>, <span class="tex-font-style-tt">aba</span>, <span class="tex-font-style-tt">abaa</span>, <span class="tex-font-style-tt">abaaa</span>}. The string <span class="tex-font-style-tt">abaa</span> has been written twice.</p><p>In the second example, Misha has written eight distinct strings: {<span class="tex-font-style-tt">aa</span>, <span class="tex-font-style-tt">aaa</span>, <span class="tex-font-style-tt">aaaa</span>, <span class="tex-font-style-tt">aaaaa</span>, <span class="tex-font-style-tt">aaaaaa</span>, <span class="tex-font-style-tt">aaaaaaa</span>, <span class="tex-font-style-tt">aaaaaaaa</span>, <span class="tex-font-style-tt">aaaaaaaaa</span>}.</p>
