## Description

<div><p>Inna loves digit <span class="tex-span">9</span> very much. That's why she asked Dima to write a small number consisting of nines. But Dima must have misunderstood her and he wrote a very large number <span class="tex-span"><i>a</i></span>, consisting of digits from <span class="tex-span">1</span> to <span class="tex-span">9</span>.</p><p>Inna wants to slightly alter the number Dima wrote so that in the end the number contained as many digits nine as possible. In one move, Inna can choose two adjacent digits in a number which sum equals <span class="tex-span">9</span> and replace them by a single digit <span class="tex-span">9</span>.</p><p>For instance, Inna can alter number <span class="tex-span">14545181</span> like this: <span class="tex-span">14545181 → 1945181 → 194519 → 19919</span>. Also, she can use this method to transform number <span class="tex-span">14545181</span> into number <span class="tex-span">19991</span>. Inna will not transform it into <span class="tex-span">149591</span> as she can get numbers <span class="tex-span">19919</span> and <span class="tex-span">19991</span> which contain more digits nine.</p><p>Dima is a programmer so he wants to find out how many distinct numbers containing as many digits nine as possible Inna can get from the written number. Help him with this challenging task.</p></div><div class="input-specification"><p>The first line of the input contains integer <span class="tex-span"><i>a</i></span> <span class="tex-span">(1 ≤ <i>a</i> ≤ 10<sup class="upper-index">100000</sup>)</span>. Number <span class="tex-span"><i>a</i></span> doesn't have any zeroes.</p></div><div class="output-specification"><p>In a single line print a single integer — the answer to the problem. It is guaranteed that the answer to the problem doesn't exceed <span class="tex-span">2<sup class="upper-index">63</sup> - 1</span>.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line of the input contains integer <span class="tex-span"><i>a</i></span> <span class="tex-span">(1 ≤ <i>a</i> ≤ 10<sup class="upper-index">100000</sup>)</span>. Number <span class="tex-span"><i>a</i></span> doesn't have any zeroes.</p>

## Output

<p>In a single line print a single integer — the answer to the problem. It is guaranteed that the answer to the problem doesn't exceed <span class="tex-span">2<sup class="upper-index">63</sup> - 1</span>.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
369727

```




```input2
123456789987654321

```




```input3
1

```




```output1
2

```




```output2
1

```




```output3
1

```



## Note

<p>Notes to the samples</p><p>In the first sample Inna can get the following numbers: <span class="tex-span">369727 → 99727 → 9997</span>, <span class="tex-span">369727 → 99727 → 9979</span>.</p><p>In the second sample, Inna can act like this: <span class="tex-span">123456789987654321 → 12396789987654321 → 1239678998769321</span>.</p>
