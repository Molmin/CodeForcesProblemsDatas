## Description

<div><p>Sengoku still remembers the mysterious "colourful meteoroids" she discovered with Lala-chan when they were little. In particular, one of the nights impressed her deeply, giving her the illusion that all her fancies would be realized.</p><p>On that night, Sengoku constructed a permutation <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> of integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> inclusive, with each integer representing a colour, wishing for the colours to see in the coming meteor outburst. Two incredible outbursts then arrived, each with <span class="tex-span"><i>n</i></span> meteorids, colours of which being integer sequences <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> respectively. Meteoroids' colours were also between <span class="tex-span">1</span> and <span class="tex-span"><i>n</i></span> inclusive, and the two sequences were not identical, that is, at least one <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) exists, such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span> holds.</p><p>Well, she almost had it all — each of the sequences <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> matched exactly <span class="tex-span"><i>n</i> - 1</span> elements in Sengoku's permutation. In other words, there is exactly one <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>p</i><sub class="lower-index"><i>i</i></sub></span>, and exactly one <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>n</i></span>) such that <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub> ≠ <i>p</i><sub class="lower-index"><i>j</i></sub></span>.</p><p>For now, Sengoku is able to recover the actual colour sequences <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> through astronomical records, but her wishes have been long forgotten. You are to reconstruct any possible permutation Sengoku could have had on that night.</p></div><div class="input-specification"><p>The first line of input contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1 000</span>) — the length of Sengoku's permutation, being the length of both meteor outbursts at the same time.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the sequence of colours in the first meteor outburst.</p><p>The third line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the sequence of colours in the second meteor outburst. At least one <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) exists, such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span> holds.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span>, denoting a possible permutation Sengoku could have had. If there are more than one possible answer, output any one of them.</p><p>Input guarantees that such permutation exists.</p></div>

## Input

<p>The first line of input contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1 000</span>) — the length of Sengoku's permutation, being the length of both meteor outbursts at the same time.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the sequence of colours in the first meteor outburst.</p><p>The third line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the sequence of colours in the second meteor outburst. At least one <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) exists, such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span> holds.</p>

## Output

<p>Output <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span>, denoting a possible permutation Sengoku could have had. If there are more than one possible answer, output any one of them.</p><p>Input guarantees that such permutation exists.</p>





```input1
5
1 2 3 4 3
1 2 5 4 5

```




```input2
5
4 4 2 3 1
5 4 5 3 1

```




```input3
4
1 1 3 4
1 4 3 4

```




```output1
1 2 5 4 3

```




```output2
5 4 2 3 1

```




```output3
1 2 3 4

```



## Note

<p>In the first sample, both <span class="tex-span">1, 2, 5, 4, 3</span> and <span class="tex-span">1, 2, 3, 4, 5</span> are acceptable outputs.</p><p>In the second sample, <span class="tex-span">5, 4, 2, 3, 1</span> is the only permutation to satisfy the constraints.</p>
