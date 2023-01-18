## Description

<div><p>Bob has a permutation of integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Denote this permutation as <span class="tex-span"><i>p</i></span>. The <span class="tex-span"><i>i</i></span>-th element of <span class="tex-span"><i>p</i></span> will be denoted as <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>. For all pairs of distinct integers <span class="tex-span"><i>i</i>, <i>j</i></span> between <span class="tex-span">1</span> and <span class="tex-span"><i>n</i></span>, he wrote the number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = <i>min</i>(<i>p</i><sub class="lower-index"><i>i</i></sub>, <i>p</i><sub class="lower-index"><i>j</i></sub>)</span>. He writes <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>i</i></sub> = 0</span> for all integer <span class="tex-span"><i>i</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p><p>Bob gave you all the values of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> that he wrote down. Your job is to reconstruct any permutation that could have generated these values. The input will be formed so that it is guaranteed that there is at least one solution that is consistent with the information given.</p></div><div class="input-specification"><p>The first line of the input will contain a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 50</span>).</p><p>The next <span class="tex-span"><i>n</i></span> lines will contain the values of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span>. The <span class="tex-span"><i>j</i></span>-th number on the <span class="tex-span"><i>i</i></span>-th line will represent <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span>. The <span class="tex-span"><i>i</i></span>-th number on the <span class="tex-span"><i>i</i></span>-th line will be <span class="tex-span">0</span>. It's guaranteed that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = <i>a</i><sub class="lower-index"><i>j</i>, <i>i</i></sub></span> and there is at least one solution consistent with the information given.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> space separated integers, which represents a permutation that could have generated these values. If there are multiple possible solutions, print any of them.</p></div>

## Input

<p>The first line of the input will contain a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 50</span>).</p><p>The next <span class="tex-span"><i>n</i></span> lines will contain the values of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span>. The <span class="tex-span"><i>j</i></span>-th number on the <span class="tex-span"><i>i</i></span>-th line will represent <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span>. The <span class="tex-span"><i>i</i></span>-th number on the <span class="tex-span"><i>i</i></span>-th line will be <span class="tex-span">0</span>. It's guaranteed that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = <i>a</i><sub class="lower-index"><i>j</i>, <i>i</i></sub></span> and there is at least one solution consistent with the information given.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> space separated integers, which represents a permutation that could have generated these values. If there are multiple possible solutions, print any of them.</p>





```input1
2
0 1
1 0

```




```input2
5
0 2 2 1 2
2 0 4 1 3
2 4 0 1 3
1 1 1 0 1
2 3 3 1 0

```




```output1
2 1

```




```output2
2 5 4 1 3

```



## Note

<p>In the first case, the answer can be <span class="tex-span">{1, 2}</span> or <span class="tex-span">{2, 1}</span>.</p><p>In the second case, another possible answer is <span class="tex-span">{2, 4, 5, 1, 3}</span>.</p>
