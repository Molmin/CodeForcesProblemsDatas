## Description

<div><p>Cosider a sequence, consisting of <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span>. Jeff can perform the following operation on sequence <span class="tex-span"><i>a</i></span>:</p><ul> <li> take three integers <span class="tex-span"><i>v</i></span>, <span class="tex-span"><i>t</i></span>, <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>v</i>, <i>t</i> ≤ <i>n</i>;&nbsp;0 ≤ <i>k</i>;&nbsp;<i>v</i> + <i>tk</i> ≤ <i>n</i>)</span>, such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>v</i></sub></span> = <span class="tex-span"><i>a</i><sub class="lower-index"><i>v</i> + <i>t</i></sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>v</i> + <i>t</i></sub></span> = <span class="tex-span"><i>a</i><sub class="lower-index"><i>v</i> + 2<i>t</i></sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>v</i> + <i>t</i>(<i>k</i> - 1)</sub></span> = <span class="tex-span"><i>a</i><sub class="lower-index"><i>v</i> + <i>tk</i></sub></span>; </li><li> remove elements <span class="tex-span"><i>a</i><sub class="lower-index"><i>v</i></sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>v</i> + <i>t</i></sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>v</i> + <i>t</i>·<i>k</i></sub></span> from the sequence <span class="tex-span"><i>a</i></span>, the remaining elements should be reindexed <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i> - <i>k</i> - 1</sub></span>. </li><li> permute in some order the remaining elements of sequence <span class="tex-span"><i>a</i></span>. </li></ul><p>A beauty of a sequence <span class="tex-span"><i>a</i></span> is the minimum number of operations that is needed to delete all elements from sequence <span class="tex-span"><i>a</i></span>.</p><p>Jeff's written down a sequence of <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>m</i></sub></span>. Now he wants to ask <span class="tex-span"><i>q</i></span> questions. Each question can be described with two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span>. The answer to the question is the beauty of sequence <span class="tex-span"><i>b</i><sub class="lower-index"><i>l</i><sub class="lower-index"><i>i</i></sub></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>l</i><sub class="lower-index"><i>i</i></sub> + 1</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>r</i><sub class="lower-index"><i>i</i></sub></sub></span>. You are given the sequence <span class="tex-span"><i>b</i></span> and all questions. Help Jeff, answer all his questions.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The next line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>m</i></sub></span> <span class="tex-span">(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span>. </p><p>The third line contains integer <span class="tex-span"><i>q</i></span> <span class="tex-span">(1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of questions. The next <span class="tex-span"><i>q</i></span> lines contain pairs of integers, <span class="tex-span"><i>i</i></span>-th of them contains a pair of integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i>)</span> — the description of <span class="tex-span"><i>i</i></span>-th question.</p></div><div class="output-specification"><p>In <span class="tex-span"><i>q</i></span> lines print the answers to Jeff's queries. Print the answers according to the order of questions in input.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The next line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>m</i></sub></span> <span class="tex-span">(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span>. </p><p>The third line contains integer <span class="tex-span"><i>q</i></span> <span class="tex-span">(1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of questions. The next <span class="tex-span"><i>q</i></span> lines contain pairs of integers, <span class="tex-span"><i>i</i></span>-th of them contains a pair of integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i>)</span> — the description of <span class="tex-span"><i>i</i></span>-th question.</p>

## Output

<p>In <span class="tex-span"><i>q</i></span> lines print the answers to Jeff's queries. Print the answers according to the order of questions in input.</p>





```input1
5
2 2 1 1 2
5
1 5
1 1
2 2
1 3
2 3

```




```input2
10
2 1 3 3 3 3 1 3 1 1
10
4 8
2 10
1 10
4 4
1 3
2 4
6 7
1 9
2 5
1 1

```




```output1
2
1
1
2
2

```




```output2
2
3
3
1
3
2
2
3
2
1

```


