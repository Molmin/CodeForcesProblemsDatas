## Description

<div><p>You are given <span class="tex-span"><i>n</i></span> <span class="tex-span"><i>k</i></span>-digit integers. You have to rearrange the digits in the integers so that the difference between the largest and the smallest number was minimum. Digits should be rearranged by the same rule in all integers.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> — the number and digit capacity of numbers correspondingly (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 8</span>). Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>k</i></span>-digit positive integers. Leading zeroes are allowed both in the initial integers and the integers resulting from the rearranging of digits.</p></div><div class="output-specification"><p>Print a single number: the minimally possible difference between the largest and the smallest number after the digits are rearranged in all integers by the same rule.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> — the number and digit capacity of numbers correspondingly (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 8</span>). Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>k</i></span>-digit positive integers. Leading zeroes are allowed both in the initial integers and the integers resulting from the rearranging of digits.</p>

## Output

<p>Print a single number: the minimally possible difference between the largest and the smallest number after the digits are rearranged in all integers by the same rule.</p>





```input1
6 4
5237
2753
7523
5723
5327
2537

```




```input2
3 3
010
909
012

```




```input3
7 5
50808
36603
37198
44911
29994
42543
50156

```




```output1
2700

```




```output2
3

```




```output3
20522

```



## Note

<p>In the first sample, if we rearrange the digits in numbers as (3,1,4,2), then the 2-nd and the 4-th numbers will equal 5237 and 2537 correspondingly (they will be maximum and minimum for such order of digits).</p><p>In the second sample, if we swap the second digits and the first ones, we get integers 100, 99 and 102.</p>
