## Description

<div><p><span class="tex-font-style-it">Right now she actually isn't. But she will be, if you don't solve this problem.</span></p><p>You are given integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span>. There is a number <span class="tex-span"><i>x</i></span>, which is initially equal to <span class="tex-span"><i>n</i></span>. You are allowed to perform two types of operations: </p><ol> <li> Subtract 1 from <span class="tex-span"><i>x</i></span>. This operation costs you <span class="tex-span"><i>A</i></span> coins. </li><li> Divide <span class="tex-span"><i>x</i></span> by <span class="tex-span"><i>k</i></span>. Can be performed only if <span class="tex-span"><i>x</i></span> is divisible by <span class="tex-span"><i>k</i></span>. This operation costs you <span class="tex-span"><i>B</i></span> coins. </li></ol> What is the minimum amount of coins you have to pay to make <span class="tex-span"><i>x</i></span> equal to <span class="tex-span">1</span>?</div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">9</sup></span>).</p><p>The second line contains a single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 2·10<sup class="upper-index">9</sup></span>).</p><p>The third line contains a single integer <span class="tex-span"><i>A</i></span> (<span class="tex-span">1 ≤ <i>A</i> ≤ 2·10<sup class="upper-index">9</sup></span>).</p><p>The fourth line contains a single integer <span class="tex-span"><i>B</i></span> (<span class="tex-span">1 ≤ <i>B</i> ≤ 2·10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Output a single integer&nbsp;— the minimum amount of coins you have to pay to make <span class="tex-span"><i>x</i></span> equal to <span class="tex-span">1</span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">9</sup></span>).</p><p>The second line contains a single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 2·10<sup class="upper-index">9</sup></span>).</p><p>The third line contains a single integer <span class="tex-span"><i>A</i></span> (<span class="tex-span">1 ≤ <i>A</i> ≤ 2·10<sup class="upper-index">9</sup></span>).</p><p>The fourth line contains a single integer <span class="tex-span"><i>B</i></span> (<span class="tex-span">1 ≤ <i>B</i> ≤ 2·10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Output a single integer&nbsp;— the minimum amount of coins you have to pay to make <span class="tex-span"><i>x</i></span> equal to <span class="tex-span">1</span>.</p>





```input1
9
2
3
1

```




```input2
5
5
2
20

```




```input3
19
3
4
2

```




```output1
6

```




```output2
8

```




```output3
12

```



## Note

<p>In the first testcase, the optimal strategy is as follows: </p><ul> <li> Subtract 1 from <span class="tex-span"><i>x</i></span> (<span class="tex-span">9 → 8</span>) paying 3 coins. </li><li> Divide <span class="tex-span"><i>x</i></span> by 2 (<span class="tex-span">8 → 4</span>) paying 1 coin. </li><li> Divide <span class="tex-span"><i>x</i></span> by 2 (<span class="tex-span">4 → 2</span>) paying 1 coin. </li><li> Divide <span class="tex-span"><i>x</i></span> by 2 (<span class="tex-span">2 → 1</span>) paying 1 coin. </li></ul><p>The total cost is <span class="tex-span">6</span> coins.</p><p>In the second test case the optimal strategy is to subtract 1 from <span class="tex-span"><i>x</i></span> <span class="tex-span">4</span> times paying <span class="tex-span">8</span> coins in total.</p>
