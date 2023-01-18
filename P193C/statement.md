## Description

<div><p><span class="tex-font-style-it">Hamming distance</span> between strings <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> of equal length (denoted by <span class="tex-span"><i>h</i>(<i>a</i>, <i>b</i>)</span>) is equal to the number of distinct integers <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ |<i>a</i>|)</span>, such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the <span class="tex-span"><i>i</i></span>-th symbol of string <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is the <span class="tex-span"><i>i</i></span>-th symbol of string <span class="tex-span"><i>b</i></span>. For example, the Hamming distance between strings "<span class="tex-font-style-tt">aba</span>" and "<span class="tex-font-style-tt">bba</span>" equals <span class="tex-span">1</span>, they have different first symbols. For strings "<span class="tex-font-style-tt">bbba</span>" and "<span class="tex-font-style-tt">aaab</span>" the Hamming distance equals <span class="tex-span">4</span>.</p><p>John Doe had a paper on which four strings of equal length <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index">3</sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index">4</sub></span> were written. Each string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> consisted only of lowercase letters "<span class="tex-font-style-tt">a</span>" and "<span class="tex-font-style-tt">b</span>". John found the Hamming distances between all pairs of strings he had. Then he lost the paper with the strings but he didn't lose the Hamming distances between all pairs.</p><p>Help John restore the strings; find some four strings <span class="tex-span"><i>s</i>'<sub class="lower-index">1</sub></span>, <span class="tex-span"><i>s</i>'<sub class="lower-index">2</sub></span>, <span class="tex-span"><i>s</i>'<sub class="lower-index">3</sub>, <i>s</i>'<sub class="lower-index">4</sub></span> of equal length that consist only of lowercase letters "<span class="tex-font-style-tt">a</span>" and "<span class="tex-font-style-tt">b</span>", such that the pairwise Hamming distances between them are the same as between John's strings. More formally, set <span class="tex-span"><i>s</i>'<sub class="lower-index"><i>i</i></sub></span> must satisfy the condition <img align="middle" class="tex-formula" src="file://d0OTnWHy.png" style="max-width: 100.0%;max-height: 100.0%;">. </p><p>To make the strings easier to put down on a piece of paper, you should choose among all suitable sets of strings the one that has strings of <span class="tex-font-style-bf">minimum length</span>. </p></div><div class="input-specification"><p>The first line contains space-separated integers <span class="tex-span"><i>h</i>(<i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>)</span>, <span class="tex-span"><i>h</i>(<i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">3</sub>)</span>, <span class="tex-span"><i>h</i>(<i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">4</sub>)</span>. The second line contains space-separated integers <span class="tex-span"><i>h</i>(<i>s</i><sub class="lower-index">2</sub>, <i>s</i><sub class="lower-index">3</sub>)</span> and <span class="tex-span"><i>h</i>(<i>s</i><sub class="lower-index">2</sub>, <i>s</i><sub class="lower-index">4</sub>)</span>. The third line contains the single integer <span class="tex-span"><i>h</i>(<i>s</i><sub class="lower-index">3</sub>, <i>s</i><sub class="lower-index">4</sub>)</span>.</p><p>All given integers <span class="tex-span"><i>h</i>(<i>s</i><sub class="lower-index"><i>i</i></sub>, <i>s</i><sub class="lower-index"><i>j</i></sub>)</span> are non-negative and do not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>. It is guaranteed that at least one number <span class="tex-span"><i>h</i>(<i>s</i><sub class="lower-index"><i>i</i></sub>, <i>s</i><sub class="lower-index"><i>j</i></sub>)</span> is positive.</p></div><div class="output-specification"><p>Print -1 if there's no suitable set of strings.</p><p>Otherwise print on the first line number <span class="tex-span"><i>len</i></span> — the length of each string. On the <span class="tex-span"><i>i</i></span>-th of the next four lines print string <span class="tex-span"><i>s</i>'<sub class="lower-index"><i>i</i></sub></span>. If there are multiple sets with the minimum length of the strings, print any of them. </p></div>

## Input

<p>The first line contains space-separated integers <span class="tex-span"><i>h</i>(<i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>)</span>, <span class="tex-span"><i>h</i>(<i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">3</sub>)</span>, <span class="tex-span"><i>h</i>(<i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">4</sub>)</span>. The second line contains space-separated integers <span class="tex-span"><i>h</i>(<i>s</i><sub class="lower-index">2</sub>, <i>s</i><sub class="lower-index">3</sub>)</span> and <span class="tex-span"><i>h</i>(<i>s</i><sub class="lower-index">2</sub>, <i>s</i><sub class="lower-index">4</sub>)</span>. The third line contains the single integer <span class="tex-span"><i>h</i>(<i>s</i><sub class="lower-index">3</sub>, <i>s</i><sub class="lower-index">4</sub>)</span>.</p><p>All given integers <span class="tex-span"><i>h</i>(<i>s</i><sub class="lower-index"><i>i</i></sub>, <i>s</i><sub class="lower-index"><i>j</i></sub>)</span> are non-negative and do not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>. It is guaranteed that at least one number <span class="tex-span"><i>h</i>(<i>s</i><sub class="lower-index"><i>i</i></sub>, <i>s</i><sub class="lower-index"><i>j</i></sub>)</span> is positive.</p>

## Output

<p>Print -1 if there's no suitable set of strings.</p><p>Otherwise print on the first line number <span class="tex-span"><i>len</i></span> — the length of each string. On the <span class="tex-span"><i>i</i></span>-th of the next four lines print string <span class="tex-span"><i>s</i>'<sub class="lower-index"><i>i</i></sub></span>. If there are multiple sets with the minimum length of the strings, print any of them. </p>





```input1
4 4 4
4 4
4

```




```output1
6
aaaabb
aabbaa
bbaaaa
bbbbbb

```


