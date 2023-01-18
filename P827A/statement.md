## Description

<div><p>Ivan had string <span class="tex-span"><i>s</i></span> consisting of small English letters. However, his friend Julia decided to make fun of him and hid the string <span class="tex-span"><i>s</i></span>. Ivan preferred making a new string to finding the old one. </p><p>Ivan knows some information about the string <span class="tex-span"><i>s</i></span>. Namely, he remembers, that string <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> occurs in string <span class="tex-span"><i>s</i></span> at least <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> times or more, he also remembers exactly <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> positions where the string <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> occurs in string <span class="tex-span"><i>s</i></span>: these positions are <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>x</i><sub class="lower-index"><i>i</i>, 2</sub>, ..., <i>x</i><sub class="lower-index"><i>i</i>, <i>k</i><sub class="lower-index"><i>i</i></sub></sub></span>. He remembers <span class="tex-span"><i>n</i></span> such strings <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>You are to reconstruct <span class="tex-font-style-bf">lexicographically minimal</span> string <span class="tex-span"><i>s</i></span> such that it fits all the information Ivan remembers. Strings <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> and string <span class="tex-span"><i>s</i></span> consist of small English letters only.</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of strings Ivan remembers.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain information about the strings. The <span class="tex-span"><i>i</i></span>-th of these lines contains non-empty string <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, then positive integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>, which equal to the number of times the string <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> occurs in string <span class="tex-span"><i>s</i></span>, and then <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> distinct positive integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>x</i><sub class="lower-index"><i>i</i>, 2</sub>, ..., <i>x</i><sub class="lower-index"><i>i</i>, <i>k</i><sub class="lower-index"><i>i</i></sub></sub></span> in increasing order — positions, in which occurrences of the string <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> in the string <span class="tex-span"><i>s</i></span> start. It is guaranteed that the sum of lengths of strings <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> doesn't exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>, <span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>, and the sum of all <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> doesn't exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>. The strings <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> can coincide.</p><p>It is guaranteed that the input data is not self-contradictory, and thus at least one answer <span class="tex-font-style-bf">always</span> exists.</p></div><div class="output-specification"><p>Print lexicographically minimal string that fits all the information Ivan remembers. </p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of strings Ivan remembers.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain information about the strings. The <span class="tex-span"><i>i</i></span>-th of these lines contains non-empty string <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, then positive integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>, which equal to the number of times the string <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> occurs in string <span class="tex-span"><i>s</i></span>, and then <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> distinct positive integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>x</i><sub class="lower-index"><i>i</i>, 2</sub>, ..., <i>x</i><sub class="lower-index"><i>i</i>, <i>k</i><sub class="lower-index"><i>i</i></sub></sub></span> in increasing order — positions, in which occurrences of the string <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> in the string <span class="tex-span"><i>s</i></span> start. It is guaranteed that the sum of lengths of strings <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> doesn't exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>, <span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>, and the sum of all <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> doesn't exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>. The strings <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> can coincide.</p><p>It is guaranteed that the input data is not self-contradictory, and thus at least one answer <span class="tex-font-style-bf">always</span> exists.</p>

## Output

<p>Print lexicographically minimal string that fits all the information Ivan remembers. </p>





```input1
3
a 4 1 3 5 7
ab 2 1 5
ca 1 4

```




```input2
1
a 1 3

```




```input3
3
ab 1 1
aba 1 3
ab 2 3 5

```




```output1
abacaba

```




```output2
aaa

```




```output3
ababab

```


