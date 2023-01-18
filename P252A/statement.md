## Description

<div><p>Little Petya likes arrays that consist of non-negative integers a lot. Recently his mom has presented him one such array consisting of <span class="tex-span"><i>n</i></span> elements. Petya immediately decided to find there a segment of consecutive elements, such that the <span class="tex-span"><i>xor</i></span> of all numbers from this segment was maximal possible. Help him with that.</p><p>The <span class="tex-span"><i>xor</i></span> operation is the bitwise exclusive "<span class="tex-font-style-tt">OR</span>", that is denoted as "<span class="tex-font-style-tt">xor</span>" in Pascal and "<span class="tex-font-style-tt">^</span>" in C/C++/Java.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of elements in the array. The second line contains the space-separated integers from the array. All numbers are non-negative integers strictly less than <span class="tex-span">2<sup class="upper-index">30</sup></span>.</p></div><div class="output-specification"><p>Print a single integer — the required maximal <span class="tex-span"><i>xor</i></span> of a segment of consecutive elements.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of elements in the array. The second line contains the space-separated integers from the array. All numbers are non-negative integers strictly less than <span class="tex-span">2<sup class="upper-index">30</sup></span>.</p>

## Output

<p>Print a single integer — the required maximal <span class="tex-span"><i>xor</i></span> of a segment of consecutive elements.</p>





```input1
5
1 2 1 1 2

```




```input2
3
1 2 7

```




```input3
4
4 2 4 8

```




```output1
3

```




```output2
7

```




```output3
14

```



## Note

<p>In the first sample one of the optimal segments is the segment that consists of the first and the second array elements, if we consider the array elements indexed starting from one.</p><p>The second sample contains only one optimal segment, which contains exactly one array element (element with index three).</p>
