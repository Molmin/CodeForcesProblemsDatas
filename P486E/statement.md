## Description

<div><p>The next "Data Structures and Algorithms" lesson will be about Longest Increasing Subsequence (LIS for short) of a sequence. For better understanding, Nam decided to learn it a few days before the lesson.</p><p>Nam created a sequence <span class="tex-span"><i>a</i></span> consisting of <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) elements <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>). A subsequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i><sub class="lower-index">1</sub></sub>, <i>a</i><sub class="lower-index"><i>i</i><sub class="lower-index">2</sub></sub>, ..., <i>a</i><sub class="lower-index"><i>i</i><sub class="lower-index"><i>k</i></sub></sub></span> where <span class="tex-span">1 ≤ <i>i</i><sub class="lower-index">1</sub> &lt; <i>i</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>i</i><sub class="lower-index"><i>k</i></sub> ≤ <i>n</i></span> is called increasing if <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i><sub class="lower-index">1</sub></sub> &lt; <i>a</i><sub class="lower-index"><i>i</i><sub class="lower-index">2</sub></sub> &lt; <i>a</i><sub class="lower-index"><i>i</i><sub class="lower-index">3</sub></sub> &lt; ... &lt; <i>a</i><sub class="lower-index"><i>i</i><sub class="lower-index"><i>k</i></sub></sub></span>. An increasing subsequence is called longest if it has maximum length among all increasing subsequences. </p><p>Nam realizes that a sequence may have several longest increasing subsequences. Hence, he divides all indexes <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>), into three groups:</p><ol><li> group of all <span class="tex-span"><i>i</i></span> such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> belongs to no longest increasing subsequences.</li><li> group of all <span class="tex-span"><i>i</i></span> such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> belongs to at least one <span class="tex-font-style-bf">but not every</span> longest increasing subsequence.</li><li> group of all <span class="tex-span"><i>i</i></span> such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> belongs to every longest increasing subsequence. </li></ol><p>Since the number of longest increasing subsequences of <span class="tex-span"><i>a</i></span> may be very large, categorizing process is very difficult. Your task is to help him finish this job.</p></div><div class="input-specification"><p>The first line contains the single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) denoting the number of elements of sequence <span class="tex-span"><i>a</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>).</p></div><div class="output-specification"><p>Print a string consisting of <span class="tex-span"><i>n</i></span> characters. <span class="tex-span"><i>i</i></span>-th character should be '<span class="tex-font-style-tt">1</span>', '<span class="tex-font-style-tt">2</span>' or '<span class="tex-font-style-tt">3</span>' depending on which group among listed above index <span class="tex-span"><i>i</i></span> belongs to.</p></div>

## Input

<p>The first line contains the single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) denoting the number of elements of sequence <span class="tex-span"><i>a</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>).</p>

## Output

<p>Print a string consisting of <span class="tex-span"><i>n</i></span> characters. <span class="tex-span"><i>i</i></span>-th character should be '<span class="tex-font-style-tt">1</span>', '<span class="tex-font-style-tt">2</span>' or '<span class="tex-font-style-tt">3</span>' depending on which group among listed above index <span class="tex-span"><i>i</i></span> belongs to.</p>





```input1
1
4

```




```input2
4
1 3 2 5

```




```input3
4
1 5 2 3

```




```output1
3

```




```output2
3223

```




```output3
3133

```



## Note

<p>In the second sample, sequence <span class="tex-span"><i>a</i></span> consists of 4 elements: <span class="tex-span">{<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub>, <i>a</i><sub class="lower-index">4</sub>}</span> = <span class="tex-span">{1, 3, 2, 5}</span>. Sequence <span class="tex-span"><i>a</i></span> has exactly 2 longest increasing subsequences of length 3, they are <span class="tex-span">{<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">4</sub>}</span> = <span class="tex-span">{1, 3, 5}</span> and <span class="tex-span">{<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">3</sub>, <i>a</i><sub class="lower-index">4</sub>}</span> = <span class="tex-span">{1, 2, 5}</span>.</p><p>In the third sample, sequence <span class="tex-span"><i>a</i></span> consists of 4 elements: <span class="tex-span">{<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub>, <i>a</i><sub class="lower-index">4</sub>}</span> = <span class="tex-span">{1, 5, 2, 3}</span>. Sequence <span class="tex-span"><i>a</i></span> have exactly 1 longest increasing subsequence of length 3, that is <span class="tex-span">{<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">3</sub>, <i>a</i><sub class="lower-index">4</sub>}</span> = <span class="tex-span">{1, 2, 3}</span>.</p>
