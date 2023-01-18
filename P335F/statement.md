## Description

<div><p>A nearby pie shop is having a special sale. For each pie you pay full price for, you may select one pie of a strictly lesser value to get for free. Given the prices of all the pies you wish to acquire, determine the minimum total amount you must pay for all of the pies.</p></div><div class="input-specification"><p>Input will begin with an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500000</span>), the number of pies you wish to acquire. Following this is a line with <span class="tex-span"><i>n</i></span> integers, each indicating the cost of a pie. All costs are positive integers not exceeding <span class="tex-span">10<sup class="upper-index">9</sup></span>.</p></div><div class="output-specification"><p>Print the minimum cost to acquire all the pies.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>Input will begin with an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500000</span>), the number of pies you wish to acquire. Following this is a line with <span class="tex-span"><i>n</i></span> integers, each indicating the cost of a pie. All costs are positive integers not exceeding <span class="tex-span">10<sup class="upper-index">9</sup></span>.</p>

## Output

<p>Print the minimum cost to acquire all the pies.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
6
3 4 5 3 4 5

```




```input2
5
5 5 5 5 5

```




```input3
4
309999 6000 2080 2080

```




```output1
14

```




```output2
25

```




```output3
314159

```



## Note

<p>In the first test case you can pay for a pie with cost 5 and get a pie with cost 4 for free, then pay for a pie with cost 5 and get a pie with cost 3 for free, then pay for a pie with cost 4 and get a pie with cost 3 for free.</p><p>In the second test case you have to pay full price for every pie.</p>
