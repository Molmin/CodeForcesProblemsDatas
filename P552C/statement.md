## Description

<div><p>Vanya has a scales for weighing loads and weights of masses <span class="tex-span"><i>w</i><sup class="upper-index">0</sup>, <i>w</i><sup class="upper-index">1</sup>, <i>w</i><sup class="upper-index">2</sup>, ..., <i>w</i><sup class="upper-index">100</sup></span> grams where <span class="tex-span"><i>w</i></span> is some integer not less than <span class="tex-span">2</span> (exactly one weight of each nominal value). Vanya wonders whether he can weight an item with mass <span class="tex-span"><i>m</i></span> using the given weights, if the weights can be put on both pans of the scales. Formally speaking, your task is to determine whether it is possible to place an item of mass <span class="tex-span"><i>m</i></span> and some weights on the left pan of the scales, and some weights on the right pan of the scales so that the pans of the scales were in balance.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>w</i>, <i>m</i></span> (<span class="tex-span">2 ≤ <i>w</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number defining the masses of the weights and the mass of the item.</p></div><div class="output-specification"><p>Print word '<span class="tex-font-style-tt">YES</span>' if the item can be weighted and '<span class="tex-font-style-tt">NO</span>' if it cannot.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>w</i>, <i>m</i></span> (<span class="tex-span">2 ≤ <i>w</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number defining the masses of the weights and the mass of the item.</p>

## Output

<p>Print word '<span class="tex-font-style-tt">YES</span>' if the item can be weighted and '<span class="tex-font-style-tt">NO</span>' if it cannot.</p>





```input1
3 7

```




```input2
100 99

```




```input3
100 50

```




```output1
YES

```




```output2
YES

```




```output3
NO

```



## Note

<p>Note to the first sample test. One pan can have an item of mass <span class="tex-span">7</span> and a weight of mass <span class="tex-span">3</span>, and the second pan can have two weights of masses <span class="tex-span">9</span> and <span class="tex-span">1</span>, correspondingly. Then <span class="tex-span">7 + 3 = 9 + 1</span>.</p><p>Note to the second sample test. One pan of the scales can have an item of mass <span class="tex-span">99</span> and the weight of mass <span class="tex-span">1</span>, and the second pan can have the weight of mass <span class="tex-span">100</span>.</p><p>Note to the third sample test. It is impossible to measure the weight of the item in the manner described in the input. </p>
