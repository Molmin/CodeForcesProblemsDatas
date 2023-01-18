## Description

<div><p><span class="tex-font-style-underline">Valery is very interested in magic. Magic attracts him so much that he sees it everywhere. He explains any strange and weird phenomenon through intervention of supernatural forces. But who would have thought that even in a regular array of numbers Valera manages to see something beautiful and magical.</span></p><p>Valera absolutely accidentally got a piece of ancient parchment on which an array of numbers was written. He immediately thought that the numbers in this array were not random. As a result of extensive research Valera worked out a wonderful property that a magical array should have: an array is defined as magic if its <span class="tex-font-style-bf">minimum and maximum coincide</span>.</p><p>He decided to share this outstanding discovery with you, but he asks you for help in return. Despite the tremendous intelligence and wit, Valera counts very badly and so you will have to complete his work. All you have to do is count the number of magical subarrays of the original array of numbers, written on the parchment. Subarray is defined as <span class="tex-font-style-bf">non-empty sequence of consecutive elements</span>.</p></div><div class="input-specification"><p>The first line of the input data contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The second line contains an array of original integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). </p></div><div class="output-specification"><p>Print on the single line the answer to the problem: the amount of subarrays, which are magical.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit numbers in C++. It is recommended to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams (you can also use the <span class="tex-font-style-tt">%I64d</span> specificator).</p></div>

## Input

<p>The first line of the input data contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The second line contains an array of original integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). </p>

## Output

<p>Print on the single line the answer to the problem: the amount of subarrays, which are magical.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit numbers in C++. It is recommended to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams (you can also use the <span class="tex-font-style-tt">%I64d</span> specificator).</p>





```input1
4
2 1 1 4

```




```input2
5
-2 -2 -2 0 1

```




```output1
5

```




```output2
8

```



## Note

<p>Notes to sample tests:</p><p>Magical subarrays are shown with pairs of indices [a;b] of the beginning and the end.</p><p>In the first sample: [1;1], [2;2], [3;3], [4;4], [2;3].</p><p>In the second sample: [1;1], [2;2], [3;3], [4;4], [5;5], [1;2], [2;3], [1;3]. </p>
