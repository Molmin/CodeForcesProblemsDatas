## Description

<div><p>Little Petya loves inequations. Help him find <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, such that the following two conditions are satisfied:</p><ul><li> <span class="tex-span"><i>a</i><sub class="lower-index">1</sub><sup class="upper-index">2</sup> + <i>a</i><sub class="lower-index">2</sub><sup class="upper-index">2</sup> + ... + <i>a</i><sub class="lower-index"><i>n</i></sub><sup class="upper-index">2</sup> ≥ <i>x</i></span></li><li> <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> + <i>a</i><sub class="lower-index">2</sub> + ... + <i>a</i><sub class="lower-index"><i>n</i></sub> ≤ <i>y</i></span></li></ul></div><div class="input-specification"><p>The first line contains three space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>x</i> ≤ 10<sup class="upper-index">12</sup>, 1 ≤ <i>y</i> ≤ 10<sup class="upper-index">6</sup></span>).</p><p>Please do not use the %lld specificator to read or write 64-bit integers in С++. It is recommended to use cin, cout streams or the %I64d specificator.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> positive integers that satisfy the conditions, one integer per line. If such numbers do not exist, print a single number "-1". If there are several solutions, print any of them.</p></div>

## Input

<p>The first line contains three space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>x</i> ≤ 10<sup class="upper-index">12</sup>, 1 ≤ <i>y</i> ≤ 10<sup class="upper-index">6</sup></span>).</p><p>Please do not use the %lld specificator to read or write 64-bit integers in С++. It is recommended to use cin, cout streams or the %I64d specificator.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> positive integers that satisfy the conditions, one integer per line. If such numbers do not exist, print a single number "-1". If there are several solutions, print any of them.</p>





```input1
5 15 15

```




```input2
2 3 2

```




```input3
1 99 11

```




```output1
4
4
1
1
2

```




```output2
-1

```




```output3
11

```


