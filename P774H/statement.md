## Description

<div><p>Stepan had a favorite string <span class="tex-span"><i>s</i></span> which consisted of the lowercase letters of the Latin alphabet. </p><p>After graduation, he decided to remember it, but it was a long time ago, so he can't now remember it. But Stepan remembers some information about the string, namely the sequence of integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>n</i></span> equals the length of the string <span class="tex-span"><i>s</i></span>, and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> equals the number of substrings in the string <span class="tex-span"><i>s</i></span> with the length <span class="tex-span"><i>i</i></span>, consisting of the <span class="tex-font-style-bf">same</span> letters. The substring is a sequence of consecutive characters in the string <span class="tex-span"><i>s</i></span>.</p><p>For example, if the Stepan's favorite string is equal to "<span class="tex-font-style-tt">tttesst</span>", the sequence <span class="tex-span"><i>c</i></span> looks like: <span class="tex-span"><i>c</i> = [7, 3, 1, 0, 0, 0, 0]</span>.</p><p>Stepan asks you to help to repair his favorite string <span class="tex-span"><i>s</i></span> according to the given sequence <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span>. </p></div><div class="input-specification"><p>The first line contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>) — the length of the Stepan's favorite string.</p><p>The second line contains the sequence of integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 2000</span>), where <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> equals the number of substrings of the string <span class="tex-span"><i>s</i></span> with the length <span class="tex-span"><i>i</i></span>, consisting of the same letters.</p><p>It is guaranteed that the input data is such that the answer always exists.</p></div><div class="output-specification"><p>Print the repaired Stepan's favorite string. If there are several answers, it is allowed to print any of them. The string should contain only lowercase letters of the English alphabet. </p></div>

## Input

<p>The first line contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>) — the length of the Stepan's favorite string.</p><p>The second line contains the sequence of integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 2000</span>), where <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> equals the number of substrings of the string <span class="tex-span"><i>s</i></span> with the length <span class="tex-span"><i>i</i></span>, consisting of the same letters.</p><p>It is guaranteed that the input data is such that the answer always exists.</p>

## Output

<p>Print the repaired Stepan's favorite string. If there are several answers, it is allowed to print any of them. The string should contain only lowercase letters of the English alphabet. </p>





```input1
6
6 3 1 0 0 0

```




```input2
4
4 0 0 0

```




```output1
kkrrrq
```




```output2
abcd

```



## Note

<p>In the first test Stepan's favorite string, for example, can be the string "<span class="tex-font-style-tt">kkrrrq</span>", because it contains <span class="tex-span">6</span> substrings with the length <span class="tex-span">1</span>, consisting of identical letters (they begin in positions <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">3</span>, <span class="tex-span">4</span>, <span class="tex-span">5</span> and <span class="tex-span">6</span>), <span class="tex-span">3</span> substrings with the length <span class="tex-span">2</span>, consisting of identical letters (they begin in positions <span class="tex-span">1</span>, <span class="tex-span">3</span> and <span class="tex-span">4</span>), and <span class="tex-span">1</span> substring with the length <span class="tex-span">3</span>, consisting of identical letters (it begins in the position <span class="tex-span">3</span>). </p>
