## Description

<div><p>There are three arrays <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span>. Each of them consists of <span class="tex-span"><i>n</i></span> integers. SmallY wants to find three integers <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>v</i></span>, <span class="tex-span"><i>w</i></span> <span class="tex-span">(0 ≤ <i>u</i>, <i>v</i>, <i>w</i> ≤ <i>n</i>)</span> such that the following condition holds: each number that appears in the union of <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span>, appears either in the first <span class="tex-span"><i>u</i></span> elements of <span class="tex-span"><i>a</i></span>, or in the first <span class="tex-span"><i>v</i></span> elements of <span class="tex-span"><i>b</i></span>, or in the first <span class="tex-span"><i>w</i></span> elements of <span class="tex-span"><i>c</i></span>. Of course, SmallY doesn't want to have huge numbers <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>w</i></span>, so she wants sum <span class="tex-span"><i>u</i> + <i>v</i> + <i>w</i></span> to be as small as possible.</p><p>Please, help her to find the minimal possible sum of <span class="tex-span"><i>u</i> + <i>v</i> + <i>w</i></span>.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> — array <span class="tex-span"><i>a</i></span>. The third line contains the description of array <span class="tex-span"><i>b</i></span> in the same format. The fourth line contains the description of array <span class="tex-span"><i>c</i></span> in the same format. The following constraint holds: <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>.</p></div><div class="output-specification"><p>Print a single integer — the minimum possible sum of <span class="tex-span"><i>u</i> + <i>v</i> + <i>w</i></span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> — array <span class="tex-span"><i>a</i></span>. The third line contains the description of array <span class="tex-span"><i>b</i></span> in the same format. The fourth line contains the description of array <span class="tex-span"><i>c</i></span> in the same format. The following constraint holds: <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>.</p>

## Output

<p>Print a single integer — the minimum possible sum of <span class="tex-span"><i>u</i> + <i>v</i> + <i>w</i></span>.</p>





```input1
3
1 1 101
1 2 1
3 2 1

```




```input2
5
1 1 2 2 3
2 2 4 3 3
3 3 1 1 1

```




```output1
5
```




```output2
5
```



## Note

<p>In the first example you should choose <span class="tex-span"><i>u</i> = 3, <i>v</i> = 0, <i>w</i> = 2</span>. </p><p>In the second example you should choose <span class="tex-span"><i>u</i> = 1, <i>v</i> = 3, <i>w</i> = 1</span>.</p>
