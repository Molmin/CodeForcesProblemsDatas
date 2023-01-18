## Description

<div><p>Devu being a small kid, likes to play a lot, but he only likes to play with arrays. While playing he came up with an interesting question which he could not solve, can you please solve it for him?</p><p>Given an array consisting of distinct integers. Is it possible to partition the whole array into <span class="tex-span"><i>k</i></span> disjoint non-empty parts such that <span class="tex-span"><i>p</i></span> of the parts have even sum (each of them must have even sum) and remaining <span class="tex-span"><i>k</i></span> - <span class="tex-span"><i>p</i></span> have odd sum? (note that parts need not to be continuous).</p><p>If it is possible to partition the array, also give any possible way of valid partitioning.</p></div><div class="input-specification"><p>The first line will contain three space separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;0 ≤ <i>p</i> ≤ <i>k</i></span>). The next line will contain <span class="tex-span"><i>n</i></span> space-separated distinct integers representing the content of array <span class="tex-span"><i>a</i></span>: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>In the first line print "<span class="tex-font-style-tt">YES</span>" (without the quotes) if it is possible to partition the array in the required way. Otherwise print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p><p>If the required partition exists, print <span class="tex-span"><i>k</i></span> lines after the first line. The <span class="tex-span"><i>i</i><sup class="upper-index"><i>th</i></sup></span> of them should contain the content of the <span class="tex-span"><i>i</i><sup class="upper-index"><i>th</i></sup></span> part. Print the content of the part in the line in the following way: firstly print the number of elements of the part, then print all the elements of the part in arbitrary order. There must be exactly <span class="tex-span"><i>p</i></span> parts with even sum, each of the remaining <span class="tex-span"><i>k</i></span> - <span class="tex-span"><i>p</i></span> parts must have odd sum.</p><p>As there can be multiple partitions, you are allowed to print any valid partition.</p></div>

## Input

<p>The first line will contain three space separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;0 ≤ <i>p</i> ≤ <i>k</i></span>). The next line will contain <span class="tex-span"><i>n</i></span> space-separated distinct integers representing the content of array <span class="tex-span"><i>a</i></span>: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>In the first line print "<span class="tex-font-style-tt">YES</span>" (without the quotes) if it is possible to partition the array in the required way. Otherwise print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p><p>If the required partition exists, print <span class="tex-span"><i>k</i></span> lines after the first line. The <span class="tex-span"><i>i</i><sup class="upper-index"><i>th</i></sup></span> of them should contain the content of the <span class="tex-span"><i>i</i><sup class="upper-index"><i>th</i></sup></span> part. Print the content of the part in the line in the following way: firstly print the number of elements of the part, then print all the elements of the part in arbitrary order. There must be exactly <span class="tex-span"><i>p</i></span> parts with even sum, each of the remaining <span class="tex-span"><i>k</i></span> - <span class="tex-span"><i>p</i></span> parts must have odd sum.</p><p>As there can be multiple partitions, you are allowed to print any valid partition.</p>





```input1
5 5 3
2 6 10 5 9

```




```input2
5 5 3
7 14 2 9 5

```




```input3
5 3 1
1 2 3 7 5

```




```output1
YES
1 9
1 5
1 10
1 6
1 2

```




```output2
NO

```




```output3
YES
3 5 1 3
1 7
1 2

```


