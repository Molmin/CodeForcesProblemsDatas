## Description

<div><p>You are given <span class="tex-span"><i>n</i></span> segments on the Ox-axis. You can drive a nail in any integer point on the Ox-axis line nail so, that all segments containing this point, are considered nailed down. If the nail passes through endpoint of some segment, this segment is considered to be nailed too. What is the smallest number of nails needed to nail all the segments down?</p></div><div class="input-specification"><p>The first line of the input contains single integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — amount of segments. Following <span class="tex-span"><i>n</i></span> lines contain descriptions of the segments. Each description is a pair of integer numbers — endpoints coordinates. All the coordinates don't exceed 10000 by absolute value. Segments can degenarate to points.</p></div><div class="output-specification"><p>The first line should contain one integer number — the smallest number of nails needed to nail all the segments down. The second line should contain coordinates of driven nails separated by space in any order. If the answer is not unique, output any.</p></div>

## Input

<p>The first line of the input contains single integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — amount of segments. Following <span class="tex-span"><i>n</i></span> lines contain descriptions of the segments. Each description is a pair of integer numbers — endpoints coordinates. All the coordinates don't exceed 10000 by absolute value. Segments can degenarate to points.</p>

## Output

<p>The first line should contain one integer number — the smallest number of nails needed to nail all the segments down. The second line should contain coordinates of driven nails separated by space in any order. If the answer is not unique, output any.</p>





```input1
2
0 2
2 5

```




```input2
5
0 3
4 2
4 8
8 10
7 7

```




```output1
1
2
```




```output2
3
7 10 3

```


