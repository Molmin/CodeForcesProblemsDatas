## Description

<div><p>Pasha has a wooden stick of some positive integer length <span class="tex-span"><i>n</i></span>. He wants to perform exactly three cuts to get four parts of the stick. Each part must have some positive integer length and the sum of these lengths will obviously be <span class="tex-span"><i>n</i></span>. </p><p>Pasha likes rectangles but hates squares, so he wonders, how many ways are there to split a stick into four parts so that it's possible to form a rectangle using these parts, but is impossible to form a square.</p><p>Your task is to help Pasha and count the number of such ways. Two ways to cut the stick are considered distinct if there exists some integer <span class="tex-span"><i>x</i></span>, such that the number of parts of length <span class="tex-span"><i>x</i></span> in the first way differ from the number of parts of length <span class="tex-span"><i>x</i></span> in the second way.</p></div><div class="input-specification"><p>The first line of the input contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">9</sup></span>) — the length of Pasha's stick.</p></div><div class="output-specification"><p>The output should contain a single integer&nbsp;— the number of ways to split Pasha's stick into four parts of positive integer length so that it's possible to make a rectangle by connecting the ends of these parts, but is impossible to form a square. </p></div>

## Input

<p>The first line of the input contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">9</sup></span>) — the length of Pasha's stick.</p>

## Output

<p>The output should contain a single integer&nbsp;— the number of ways to split Pasha's stick into four parts of positive integer length so that it's possible to make a rectangle by connecting the ends of these parts, but is impossible to form a square. </p>





```input1
6

```




```input2
20

```




```output1
1

```




```output2
4

```



## Note

<p>There is only one way to divide the stick in the first sample {1, 1, 2, 2}.</p><p>Four ways to divide the stick in the second sample are {1, 1, 9, 9}, {2, 2, 8, 8}, {3, 3, 7, 7} and {4, 4, 6, 6}. Note that {5, 5, 5, 5} doesn't work.</p>
