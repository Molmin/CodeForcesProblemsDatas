## Description

<div><p>Little Petya very much likes arrays consisting of <span class="tex-span"><i>n</i></span> integers, where each of them is in the range from <span class="tex-span">1</span> to <span class="tex-span">10<sup class="upper-index">9</sup></span>, inclusive. Recently he has received one such array as a gift from his mother. Petya didn't like it at once. He decided to choose exactly one element from the array and replace it with another integer that also lies in the range from <span class="tex-span">1</span> to <span class="tex-span">10<sup class="upper-index">9</sup></span>, inclusive. It is <span class="tex-font-style-bf">not allowed</span> to replace a number with itself or to change no number at all. </p><p>After the replacement Petya sorted the array by the numbers' non-decreasing. Now he wants to know for each position: what minimum number could occupy it after the replacement and the sorting.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), which represents how many numbers the array has. The next line contains <span class="tex-span"><i>n</i></span> space-separated integers — the array's description. All elements of the array lie in the range from <span class="tex-span">1</span> to <span class="tex-span">10<sup class="upper-index">9</sup></span>, inclusive.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> space-separated integers — the minimum possible values of each array element after one replacement and the sorting are performed.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), which represents how many numbers the array has. The next line contains <span class="tex-span"><i>n</i></span> space-separated integers — the array's description. All elements of the array lie in the range from <span class="tex-span">1</span> to <span class="tex-span">10<sup class="upper-index">9</sup></span>, inclusive.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> space-separated integers — the minimum possible values of each array element after one replacement and the sorting are performed.</p>





```input1
5
1 2 3 4 5

```




```input2
5
2 3 4 5 6

```




```input3
3
2 2 2

```




```output1
1 1 2 3 4

```




```output2
1 2 3 4 5

```




```output3
1 2 2

```


