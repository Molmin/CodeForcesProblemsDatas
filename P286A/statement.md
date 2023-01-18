## Description

<div><p>A permutation <span class="tex-span"><i>p</i></span> of size <span class="tex-span"><i>n</i></span> is the sequence <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span>, consisting of <span class="tex-span"><i>n</i></span> distinct integers, each of them is from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>.</p><p>A lucky permutation is such permutation <span class="tex-span"><i>p</i></span>, that any integer <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>n</i>)</span> meets this condition <span class="tex-span"><i>p</i><sub class="lower-index"><i>p</i><sub class="lower-index"><i>i</i></sub></sub> = <i>n</i> - <i>i</i> + 1</span>.</p><p>You have integer <span class="tex-span"><i>n</i></span>. Find some lucky permutation <span class="tex-span"><i>p</i></span> of size <span class="tex-span"><i>n</i></span>.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the required permutation size.</p></div><div class="output-specification"><p>Print "-1" (without the quotes) if the lucky permutation <span class="tex-span"><i>p</i></span> of size <span class="tex-span"><i>n</i></span> doesn't exist.</p><p>Otherwise, print <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> after a space — the required permutation.</p><p>If there are multiple answers, you can print any of them.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the required permutation size.</p>

## Output

<p>Print "-1" (without the quotes) if the lucky permutation <span class="tex-span"><i>p</i></span> of size <span class="tex-span"><i>n</i></span> doesn't exist.</p><p>Otherwise, print <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> after a space — the required permutation.</p><p>If there are multiple answers, you can print any of them.</p>





```input1
1

```




```input2
2

```




```input3
4

```




```input4
5

```




```output1
1 

```




```output2
-1

```




```output3
2 4 1 3 

```




```output4
2 5 3 1 4 

```


