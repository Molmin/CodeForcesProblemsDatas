## Description

<div><p>You are given a sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> consisting of <span class="tex-font-style-bf">different</span> integers. It is required to split this sequence into the <span class="tex-font-style-bf">maximum</span> number of subsequences such that after sorting integers in each of them in increasing order, the total sequence also will be sorted in increasing order.</p><p>Sorting integers in a subsequence is a process such that the numbers included in a subsequence are ordered in increasing order, and the numbers which are not included in a subsequence don't change their places.</p><p>Every element of the sequence must appear in exactly one subsequence.</p></div><div class="input-specification"><p>The first line of input data contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the length of the sequence.</p><p>The second line of input data contains <span class="tex-span"><i>n</i></span> different integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the elements of the sequence. It is guaranteed that all elements of the sequence are distinct.</p></div><div class="output-specification"><p>In the first line print the maximum number of subsequences <span class="tex-span"><i>k</i></span>, which the original sequence can be split into while fulfilling the requirements.</p><p>In the next <span class="tex-span"><i>k</i></span> lines print the description of subsequences in the following format: the number of elements in subsequence <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 &lt; <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), then <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> integers <span class="tex-span"><i>l</i><sub class="lower-index">1</sub>, <i>l</i><sub class="lower-index">2</sub>, ..., <i>l</i><sub class="lower-index"><i>c</i><sub class="lower-index"><i>i</i></sub></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>)&nbsp;— indices of these elements in the original sequence. </p><p>Indices could be printed in any order. Every index from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> must appear in output <span class="tex-font-style-bf">exactly once</span>.</p><p>If there are several possible answers, print any of them.</p></div>

## Input

<p>The first line of input data contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the length of the sequence.</p><p>The second line of input data contains <span class="tex-span"><i>n</i></span> different integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the elements of the sequence. It is guaranteed that all elements of the sequence are distinct.</p>

## Output

<p>In the first line print the maximum number of subsequences <span class="tex-span"><i>k</i></span>, which the original sequence can be split into while fulfilling the requirements.</p><p>In the next <span class="tex-span"><i>k</i></span> lines print the description of subsequences in the following format: the number of elements in subsequence <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 &lt; <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), then <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> integers <span class="tex-span"><i>l</i><sub class="lower-index">1</sub>, <i>l</i><sub class="lower-index">2</sub>, ..., <i>l</i><sub class="lower-index"><i>c</i><sub class="lower-index"><i>i</i></sub></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>)&nbsp;— indices of these elements in the original sequence. </p><p>Indices could be printed in any order. Every index from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> must appear in output <span class="tex-font-style-bf">exactly once</span>.</p><p>If there are several possible answers, print any of them.</p>





```input1
6
3 2 1 6 5 4

```




```input2
6
83 -75 -49 11 37 62

```




```output1
4
2 1 3
1 2
2 4 6
1 5

```




```output2
1
6 1 2 3 4 5 6

```



## Note

<p>In the first sample output:</p><p>After sorting the first subsequence we will get sequence <span class="tex-span">1&nbsp;2&nbsp;3&nbsp;6&nbsp;5&nbsp;4</span>.</p><p>Sorting the second subsequence changes nothing.</p><p>After sorting the third subsequence we will get sequence <span class="tex-span">1&nbsp;2&nbsp;3&nbsp;4&nbsp;5&nbsp;6</span>.</p><p>Sorting the last subsequence changes nothing.</p>
