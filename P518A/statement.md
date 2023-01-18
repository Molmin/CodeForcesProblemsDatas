## Description

<div><p>Vitaly is a diligent student who never missed a lesson in his five years of studying in the university. He always does his homework on time and passes his exams in time. </p><p>During the last lesson the teacher has provided two strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> to Vitaly. The strings have the same length, they consist of lowercase English letters, string <span class="tex-span"><i>s</i></span> is lexicographically smaller than string <span class="tex-span"><i>t</i></span>. Vitaly wondered if there is such string that is lexicographically larger than string <span class="tex-span"><i>s</i></span> and at the same is lexicographically smaller than string <span class="tex-span"><i>t</i></span>. This string should also consist of lowercase English letters and have the length equal to the lengths of strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>. </p><p>Let's help Vitaly solve this easy problem!</p></div><div class="input-specification"><p>The first line contains string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 100</span>), consisting of lowercase English letters. Here, <span class="tex-span">|<i>s</i>|</span> denotes the length of the string.</p><p>The second line contains string <span class="tex-span"><i>t</i></span> (<span class="tex-span">|<i>t</i>| = |<i>s</i>|</span>), consisting of lowercase English letters.</p><p>It is guaranteed that the lengths of strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> are the same and string <span class="tex-span"><i>s</i></span> is lexicographically less than string <span class="tex-span"><i>t</i></span>.</p></div><div class="output-specification"><p>If the string that meets the given requirements doesn't exist, print a single string "<span class="tex-font-style-tt">No such string</span>" (without the quotes).</p><p>If such string exists, print it. If there are multiple valid strings, you may print any of them.</p></div>

## Input

<p>The first line contains string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 100</span>), consisting of lowercase English letters. Here, <span class="tex-span">|<i>s</i>|</span> denotes the length of the string.</p><p>The second line contains string <span class="tex-span"><i>t</i></span> (<span class="tex-span">|<i>t</i>| = |<i>s</i>|</span>), consisting of lowercase English letters.</p><p>It is guaranteed that the lengths of strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> are the same and string <span class="tex-span"><i>s</i></span> is lexicographically less than string <span class="tex-span"><i>t</i></span>.</p>

## Output

<p>If the string that meets the given requirements doesn't exist, print a single string "<span class="tex-font-style-tt">No such string</span>" (without the quotes).</p><p>If such string exists, print it. If there are multiple valid strings, you may print any of them.</p>





```input1
a
c

```




```input2
aaa
zzz

```




```input3
abcdefg
abcdefh

```




```output1
b

```




```output2
kkk

```




```output3
No such string

```



## Note

<p>String <span class="tex-span"><i>s</i> = <i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index"><i>n</i></sub></span> is said to be lexicographically smaller than <span class="tex-span"><i>t</i> = <i>t</i><sub class="lower-index">1</sub><i>t</i><sub class="lower-index">2</sub>... <i>t</i><sub class="lower-index"><i>n</i></sub></span>, if there exists such <span class="tex-span"><i>i</i></span>, that <span class="tex-span"><i>s</i><sub class="lower-index">1</sub> = <i>t</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub> = <i>t</i><sub class="lower-index">2</sub>, ... <i>s</i><sub class="lower-index"><i>i</i> - 1</sub> = <i>t</i><sub class="lower-index"><i>i</i> - 1</sub>, <i>s</i><sub class="lower-index"><i>i</i></sub> &lt; <i>t</i><sub class="lower-index"><i>i</i></sub></span>.</p>
