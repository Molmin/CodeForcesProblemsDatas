## Description

<div><p>The sequence is called <span class="tex-font-style-underline">ordered</span> if it is non-decreasing or non-increasing. For example, sequnces [3, 1, 1, 0] and [1, 2, 3, 100] are ordered, but the sequence [1, 3, 3, 1] is not. You are given a sequence of numbers. You are to find it's shortest subsequence which is not ordered.</p><p>A subsequence is a sequence that can be derived from the given sequence by deleting zero or more elements without changing the order of the remaining elements.</p></div><div class="input-specification"><p>The first line of the input contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The second line contains <span class="tex-span"><i>n</i></span> space-separated integers — the given sequence. All numbers in this sequence do not exceed <span class="tex-span">10<sup class="upper-index">6</sup></span> by absolute value.</p></div><div class="output-specification"><p>If the given sequence does not contain any unordered subsequences, output <span class="tex-span">0</span>. Otherwise, output the length <span class="tex-span"><i>k</i></span> of the shortest such subsequence. Then output <span class="tex-span"><i>k</i></span> integers from the range [1..<span class="tex-span"><i>n</i></span>] — indexes of the elements of this subsequence. If there are several solutions, output any of them.</p></div>

## Input

<p>The first line of the input contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The second line contains <span class="tex-span"><i>n</i></span> space-separated integers — the given sequence. All numbers in this sequence do not exceed <span class="tex-span">10<sup class="upper-index">6</sup></span> by absolute value.</p>

## Output

<p>If the given sequence does not contain any unordered subsequences, output <span class="tex-span">0</span>. Otherwise, output the length <span class="tex-span"><i>k</i></span> of the shortest such subsequence. Then output <span class="tex-span"><i>k</i></span> integers from the range [1..<span class="tex-span"><i>n</i></span>] — indexes of the elements of this subsequence. If there are several solutions, output any of them.</p>





```input1
5
67 499 600 42 23

```




```input2
3
1 2 3

```




```input3
3
2 3 1

```




```output1
3
1 3 5

```




```output2
0

```




```output3
3
1 2 3

```


