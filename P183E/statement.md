## Description

<div><p>The prestigious Codeforces kindergarten consists of <span class="tex-span"><i>n</i></span> kids, numbered <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span>. Each of them are given allowance in rubles by their parents.</p><p>Today, they are going to the most famous candy shop in the town. The shop sells candies in packages: for all <span class="tex-span"><i>i</i></span> between <span class="tex-span">1</span> and <span class="tex-span"><i>m</i></span>, inclusive, it sells a package containing exactly <span class="tex-span"><i>i</i></span> candies. A candy costs one ruble, so a package containing <span class="tex-span"><i>x</i></span> candies costs <span class="tex-span"><i>x</i></span> rubles.</p><p>The kids will purchase candies in turns, starting from kid 1. In a single turn, kid <span class="tex-span"><i>i</i></span> will purchase one candy package. Due to the highly competitive nature of Codeforces kindergarten, during a turn, the number of candies contained in the package purchased by the kid will always be strictly greater than the number of candies contained in the package purchased by the kid in the preceding turn (an exception is in the first turn: the first kid may purchase any package). Then, the turn proceeds to kid <span class="tex-span"><i>i</i> + 1</span>, or to kid <span class="tex-span">1</span> if it was kid <span class="tex-span"><i>n</i></span>'s turn. This process can be ended at any time, but at the end of the purchase process, all the kids <span class="tex-font-style-underline">must have the same number of candy packages</span>. Of course, the amount spent by each kid on the candies cannot exceed their allowance.</p><p>You work at the candy shop and would like to prepare the candies for the kids. Print the maximum number of candies that can be sold by the candy shop to the kids. If the kids cannot purchase any candy (due to insufficient allowance), print <span class="tex-span">0</span>.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup>, 2 ≤ <i>m</i> ≤ 5·10<sup class="upper-index">6</sup>, <i>n</i> ≤ <i>m</i></span>), denoting the number of kids and the maximum number of candies in a package sold by the candy shop, respectively.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow, each line will contain a single positive integer not exceeding <img align="middle" class="tex-formula" src="file://NDxwmZQL.png" style="max-width: 100.0%;max-height: 100.0%;"> denoting the allowance of a kid in rubles. The allowances are given in order from kid <span class="tex-span">1</span> to kid <span class="tex-span"><i>n</i></span>.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is recommended to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams (also you may use <span class="tex-font-style-tt">%I64d</span> specificator).</p></div><div class="output-specification"><p>Print a single integer denoting the maximum number of candies that can be sold by the candy shop.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup>, 2 ≤ <i>m</i> ≤ 5·10<sup class="upper-index">6</sup>, <i>n</i> ≤ <i>m</i></span>), denoting the number of kids and the maximum number of candies in a package sold by the candy shop, respectively.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow, each line will contain a single positive integer not exceeding <img align="middle" class="tex-formula" src="file://NDxwmZQL.png" style="max-width: 100.0%;max-height: 100.0%;"> denoting the allowance of a kid in rubles. The allowances are given in order from kid <span class="tex-span">1</span> to kid <span class="tex-span"><i>n</i></span>.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is recommended to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams (also you may use <span class="tex-font-style-tt">%I64d</span> specificator).</p>

## Output

<p>Print a single integer denoting the maximum number of candies that can be sold by the candy shop.</p>





```input1
2 5
5
10

```




```input2
3 8
8
16
13

```




```input3
2 5000000
12500002500000
12500002500000

```




```output1
13

```




```output2
32

```




```output3
12500002500000

```



## Note

<p>For the first example, one of the scenarios that will result in <span class="tex-span">13</span> purchased candies is as follows. </p><ul> <li> Turn 1. Kid 1 purchases 1 candy. </li><li> Turn 2. Kid 2 purchases 3 candies. </li><li> Turn 3. Kid 1 purchases 4 candies. </li><li> Turn 4. Kid 2 purchases 5 candies. </li></ul>
