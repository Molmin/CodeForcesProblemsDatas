## Description

<div><p>Little Petya loves looking for numbers' divisors. One day Petya came across the following problem:</p><p>You are given <span class="tex-span"><i>n</i></span> queries in the form "<span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>". For each query Petya should count how many divisors of number <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> divide none of the numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i> - <i>y</i><sub class="lower-index"><i>i</i></sub></sub>, <i>x</i><sub class="lower-index"><i>i</i> - <i>y</i><sub class="lower-index"><i>i</i></sub> + 1</sub>, ..., <i>x</i><sub class="lower-index"><i>i</i> - 1</sub></span>. Help him.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). Each of the following <span class="tex-span"><i>n</i></span> lines contain two space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>i</i> - 1</span>, where <span class="tex-span"><i>i</i></span> is the query's ordinal number; the numeration starts with <span class="tex-span">1</span>). </p><p>If <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub> = 0</span> for the query, then the answer to the query will be the number of divisors of the number <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>. In this case you do not need to take the previous numbers <span class="tex-span"><i>x</i></span> into consideration.</p></div><div class="output-specification"><p>For each query print the answer on a single line: the number of positive integers <span class="tex-span"><i>k</i></span> such that <img align="middle" class="tex-formula" src="file://MHuPNCBg.png" style="max-width: 100.0%;max-height: 100.0%;"></p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). Each of the following <span class="tex-span"><i>n</i></span> lines contain two space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>i</i> - 1</span>, where <span class="tex-span"><i>i</i></span> is the query's ordinal number; the numeration starts with <span class="tex-span">1</span>). </p><p>If <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub> = 0</span> for the query, then the answer to the query will be the number of divisors of the number <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>. In this case you do not need to take the previous numbers <span class="tex-span"><i>x</i></span> into consideration.</p>

## Output

<p>For each query print the answer on a single line: the number of positive integers <span class="tex-span"><i>k</i></span> such that <img align="middle" class="tex-formula" src="file://MHuPNCBg.png" style="max-width: 100.0%;max-height: 100.0%;"></p>





```input1
6
4 0
3 1
5 2
6 2
18 4
10000 3

```




```output1
3
1
1
2
2
22

```



## Note

<p>Let's write out the divisors that give answers for the first 5 queries:</p><p>1) 1, 2, 4 </p><p>2) 3</p><p>3) 5</p><p>4) 2, 6</p><p>5) 9, 18</p>
