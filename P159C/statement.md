## Description

<div><p>One popular website developed an unusual username editing procedure. One can change the username only by deleting some characters from it: to change the current name <span class="tex-span"><i>s</i></span>, a user can pick number <span class="tex-span"><i>p</i></span> and character <span class="tex-span"><i>c</i></span> and delete the <span class="tex-span"><i>p</i></span>-th occurrence of character <span class="tex-span"><i>c</i></span> from the name. After the user changed his name, he can't undo the change.</p><p>For example, one can change name "<span class="tex-font-style-tt">arca</span>" by removing the second occurrence of character "<span class="tex-font-style-tt">a</span>" to get "<span class="tex-font-style-tt">arc</span>". </p><p>Polycarpus learned that some user initially registered under nickname <span class="tex-span"><i>t</i></span>, where <span class="tex-span"><i>t</i></span> is a concatenation of <span class="tex-span"><i>k</i></span> copies of string <span class="tex-span"><i>s</i></span>. Also, Polycarpus knows the sequence of this user's name changes. Help Polycarpus figure out the user's final name.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 2000</span>). The second line contains a non-empty string <span class="tex-span"><i>s</i></span>, consisting of lowercase Latin letters, at most <span class="tex-span">100</span> characters long. The third line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 20000</span>) — the number of username changes. Each of the next <span class="tex-span"><i>n</i></span> lines contains the actual changes, one per line. The changes are written as "<span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>" (without the quotes), where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 200000</span>) is the number of occurrences of letter <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is a lowercase Latin letter. It is guaranteed that the operations are correct, that is, the letter to be deleted always exists, and after all operations not all letters are deleted from the name. The letters' occurrences are numbered starting from 1.</p></div><div class="output-specification"><p>Print a single string — the user's final name after all changes are applied to it.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 2000</span>). The second line contains a non-empty string <span class="tex-span"><i>s</i></span>, consisting of lowercase Latin letters, at most <span class="tex-span">100</span> characters long. The third line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 20000</span>) — the number of username changes. Each of the next <span class="tex-span"><i>n</i></span> lines contains the actual changes, one per line. The changes are written as "<span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>" (without the quotes), where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 200000</span>) is the number of occurrences of letter <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is a lowercase Latin letter. It is guaranteed that the operations are correct, that is, the letter to be deleted always exists, and after all operations not all letters are deleted from the name. The letters' occurrences are numbered starting from 1.</p>

## Output

<p>Print a single string — the user's final name after all changes are applied to it.</p>





```input1
2
bac
3
2 a
1 b
2 c

```




```input2
1
abacaba
4
1 a
1 a
1 c
2 b

```




```output1
acb

```




```output2
baa

```



## Note

<p>Let's consider the first sample. Initially we have name "<span class="tex-font-style-tt">bacbac</span>"; the first operation transforms it into "<span class="tex-font-style-tt">bacbc</span>", the second one — to "<span class="tex-font-style-tt">acbc</span>", and finally, the third one transforms it into "<span class="tex-font-style-tt">acb</span>".</p>
