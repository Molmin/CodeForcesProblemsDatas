## Description

<div><p>Little Petya likes positive integers a lot. Recently his mom has presented him a positive integer <span class="tex-span"><i>a</i></span>. There's only one thing Petya likes more than numbers: playing with little Masha. It turned out that Masha already has a positive integer <span class="tex-span"><i>b</i></span>. Petya decided to turn his number <span class="tex-span"><i>a</i></span> into the number <span class="tex-span"><i>b</i></span> consecutively performing the operations of the following two types:</p><ol> <li> Subtract 1 from his number. </li><li> Choose any integer <span class="tex-span"><i>x</i></span> from <span class="tex-span">2</span> to <span class="tex-span"><i>k</i></span>, inclusive. Then subtract number <span class="tex-span">(<i>a</i> <i>mod</i> <i>x</i>)</span> from his number <span class="tex-span"><i>a</i></span>. Operation <span class="tex-span"><i>a</i> <i>mod</i> <i>x</i></span> means taking the remainder from division of number <span class="tex-span"><i>a</i></span> by number <span class="tex-span"><i>x</i></span>. </li></ol><p>Petya performs one operation per second. Each time he chooses an operation to perform during the current move, no matter what kind of operations he has performed by that moment. In particular, this implies that he can perform the same operation any number of times in a row.</p><p>Now he wonders in what minimum number of seconds he could transform his number <span class="tex-span"><i>a</i></span> into number <span class="tex-span"><i>b</i></span>. Please note that numbers <span class="tex-span"><i>x</i></span> in the operations of the second type are selected anew each time, independently of each other.</p></div><div class="input-specification"><p>The only line contains three integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>b</i> ≤ <i>a</i> ≤ 10<sup class="upper-index">18</sup></span>) and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>k</i> ≤ 15</span>).</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div><div class="output-specification"><p>Print a single integer — the required minimum number of seconds needed to transform number <span class="tex-span"><i>a</i></span> into number <span class="tex-span"><i>b</i></span>.</p></div>

## Input

<p>The only line contains three integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>b</i> ≤ <i>a</i> ≤ 10<sup class="upper-index">18</sup></span>) and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>k</i> ≤ 15</span>).</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>

## Output

<p>Print a single integer — the required minimum number of seconds needed to transform number <span class="tex-span"><i>a</i></span> into number <span class="tex-span"><i>b</i></span>.</p>





```input1
10 1 4

```




```input2
6 3 10

```




```input3
1000000000000000000 1 3

```




```output1
6

```




```output2
2

```




```output3
666666666666666667

```



## Note

<p>In the first sample the sequence of numbers that Petya gets as he tries to obtain number <span class="tex-span"><i>b</i></span> is as follows: 10 <span class="tex-span"> → </span> 8 <span class="tex-span"> → </span> 6 <span class="tex-span"> → </span> 4 <span class="tex-span"> → </span> 3 <span class="tex-span"> → </span> 2 <span class="tex-span"> → </span> 1.</p><p>In the second sample one of the possible sequences is as follows: 6 <span class="tex-span"> → </span> 4 <span class="tex-span"> → </span> 3.</p>
