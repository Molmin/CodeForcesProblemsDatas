## Description

<div><p>As we communicate, we learn much new information. However, the process of communication takes too much time. It becomes clear if we look at the words we use in our everyday speech.</p><p>We can list many simple words consisting of many letters: "information", "technologies", "university", "construction", "conservatoire", "refrigerator", "stopwatch", "windowsill", "electricity", "government" and so on. Of course, we can continue listing those words ad infinitum. </p><p>Fortunately, the solution for that problem has been found. To make our speech clear and brief, we should replace the initial words with those that resemble them but are much shorter. This idea hasn't been brought into life yet, that's why you are chosen to improve the situation. </p><p>Let's consider the following formal model of transforming words: we shall assume that one can use <span class="tex-span"><i>n</i></span> words in a chat. For each words we shall introduce a notion of its shorter variant. We shall define <span class="tex-font-style-bf">shorter variant</span> of an arbitrary word <span class="tex-span"><i>s</i></span> as such word <span class="tex-span"><i>t</i></span>, that meets the following conditions:</p><ul> <li> it occurs in <span class="tex-span"><i>s</i></span> as a <span class="tex-font-style-bf">subsequence</span>, </li><li> its length ranges from one to four characters. </li></ul><p>In other words, the word <span class="tex-span"><i>t</i></span> consists at least of one and at most of four characters that occur in the same order in the word <span class="tex-span"><i>s</i></span>. Note that those characters do not necessarily follow in <span class="tex-span"><i>s</i></span> immediately one after another. You are allowed not to shorten the initial word if its length does not exceed four characters.</p><p>You are given a list of <span class="tex-span"><i>n</i></span> different words. Your task is to find a set of their shortened variants. The shortened variants of all words from the list should be different.</p></div><div class="input-specification"><p>The first line of the input file contains the only integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 200)</span>. Then <span class="tex-span"><i>n</i></span> lines contain a set of different non-empty words that consist of lowercase Latin letters. The length of each word does not exceed <span class="tex-span">10</span> characters.</p></div><div class="output-specification"><p>If the solution exists, print in the output file exactly <span class="tex-span"><i>n</i></span> lines, where the <span class="tex-span"><i>i</i></span>-th line represents the shortened variant of the <span class="tex-span"><i>i</i></span>-th word from the initial set. If there are several variants to solve the problem, print any of them. If there is no solution, print <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line of the input file contains the only integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 200)</span>. Then <span class="tex-span"><i>n</i></span> lines contain a set of different non-empty words that consist of lowercase Latin letters. The length of each word does not exceed <span class="tex-span">10</span> characters.</p>

## Output

<p>If the solution exists, print in the output file exactly <span class="tex-span"><i>n</i></span> lines, where the <span class="tex-span"><i>i</i></span>-th line represents the shortened variant of the <span class="tex-span"><i>i</i></span>-th word from the initial set. If there are several variants to solve the problem, print any of them. If there is no solution, print <span class="tex-font-style-tt">-1</span>.</p>





```input1
6
privet
spasibo
codeforces
java
marmelad
normalno

```




```input2
5
aaa
aa
a
aaaa
aaaaa

```




```output1
pret
sps
cdfs
java
mama
norm

```




```output2
-1

```


