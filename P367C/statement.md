## Description

<div><p>Let's call an array consisting of <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span>, <span class="tex-font-style-it">beautiful</span> if it has the following property:</p><ul> <li> consider all pairs of numbers <span class="tex-span"><i>x</i>, <i>y</i></span> <span class="tex-span">(<i>x</i> ≠ <i>y</i>)</span>, such that number <span class="tex-span"><i>x</i></span> occurs in the array <span class="tex-span"><i>a</i></span> and number <span class="tex-span"><i>y</i></span> occurs in the array <span class="tex-span"><i>a</i></span>; </li><li> for each pair <span class="tex-span"><i>x</i>, <i>y</i></span> must exist some position <span class="tex-span"><i>j</i></span> <span class="tex-span">(1 ≤ <i>j</i> &lt; <i>n</i>)</span>, such that at least one of the two conditions are met, either <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub> = <i>x</i>, <i>a</i><sub class="lower-index"><i>j</i> + 1</sub> = <i>y</i></span>, or <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub> = <i>y</i>, <i>a</i><sub class="lower-index"><i>j</i> + 1</sub> = <i>x</i></span>. </li></ul><p>Sereja wants to build a beautiful array <span class="tex-span"><i>a</i></span>, consisting of <span class="tex-span"><i>n</i></span> integers. But not everything is so easy, Sereja's friend Dima has <span class="tex-span"><i>m</i></span> coupons, each contains two integers <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub>, <i>w</i><sub class="lower-index"><i>i</i></sub></span>. Coupon <span class="tex-span"><i>i</i></span> costs <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> and allows you to use as many numbers <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> as you want when constructing the array <span class="tex-span"><i>a</i></span>. Values <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> are distinct. Sereja has no coupons, so Dima and Sereja have made the following deal. Dima builds some beautiful array <span class="tex-span"><i>a</i></span> of <span class="tex-span"><i>n</i></span> elements. After that he takes <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> rubles from Sereja for each <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span>, which occurs in the array <span class="tex-span"><i>a</i></span>. Sereja believed his friend and agreed to the contract, and now he is wondering, what is the maximum amount of money he can pay.</p><p>Help Sereja, find the maximum amount of money he can pay to Dima.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">6</sup>, 1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>. Next <span class="tex-span"><i>m</i></span> lines contain pairs of integers. The <span class="tex-span"><i>i</i></span>-th line contains numbers <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub>, <i>w</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>q</i><sub class="lower-index"><i>i</i></sub>, <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span>.</p><p>It is guaranteed that all <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p></div><div class="output-specification"><p>In a single line print maximum amount of money (in rubles) Sereja can pay.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">6</sup>, 1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>. Next <span class="tex-span"><i>m</i></span> lines contain pairs of integers. The <span class="tex-span"><i>i</i></span>-th line contains numbers <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub>, <i>w</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>q</i><sub class="lower-index"><i>i</i></sub>, <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span>.</p><p>It is guaranteed that all <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p>

## Output

<p>In a single line print maximum amount of money (in rubles) Sereja can pay.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
5 2
1 2
2 3

```




```input2
100 3
1 2
2 1
3 1

```




```input3
1 2
1 1
2 100

```




```output1
5

```




```output2
4

```




```output3
100

```



## Note

<p>In the first sample Sereja can pay <span class="tex-span">5</span> rubles, for example, if Dima constructs the following array: <span class="tex-span">[1, 2, 1, 2, 2]</span>. There are another optimal arrays for this test.</p><p>In the third sample Sereja can pay <span class="tex-span">100</span> rubles, if Dima constructs the following array: <span class="tex-span">[2]</span>.</p>
