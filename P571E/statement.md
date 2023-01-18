## Description

<div><p>Geometric progression with the first element <span class="tex-span"><i>a</i></span> and common ratio <span class="tex-span"><i>b</i></span> is a sequence of numbers <span class="tex-span"><i>a</i>, <i>ab</i>, <i>ab</i><sup class="upper-index">2</sup>, <i>ab</i><sup class="upper-index">3</sup>, ...</span>.</p><p>You are given <span class="tex-span"><i>n</i></span> integer geometric progressions. Your task is to find the smallest integer <span class="tex-span"><i>x</i></span>, that is the element of all the given progressions, or else state that such integer does not exist.</p></div><div class="input-specification"><p>The first line contains integer (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of geometric progressions. </p><p>Next <span class="tex-span"><i>n</i></span> lines contain pairs of integers <span class="tex-span"><i>a</i>, <i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">9</sup></span>), that are the first element and the common ratio of the corresponding geometric progression.</p></div><div class="output-specification"><p>If the intersection of all progressions is empty, then print <span class="tex-span"> - 1</span>, otherwise print the remainder of the minimal positive integer number belonging to all progressions modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div>

## Input

<p>The first line contains integer (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of geometric progressions. </p><p>Next <span class="tex-span"><i>n</i></span> lines contain pairs of integers <span class="tex-span"><i>a</i>, <i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">9</sup></span>), that are the first element and the common ratio of the corresponding geometric progression.</p>

## Output

<p>If the intersection of all progressions is empty, then print <span class="tex-span"> - 1</span>, otherwise print the remainder of the minimal positive integer number belonging to all progressions modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p>





```input1
2
2 2
4 1

```




```input2
2
2 2
3 3

```




```output1
4

```




```output2
-1

```



## Note

<p>In the second sample test one of the progressions contains only powers of two, the other one contains only powers of three.</p>
