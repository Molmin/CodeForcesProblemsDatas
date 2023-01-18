## Description

<div><p>Vitaly is a very weird man. He's got two favorite digits <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. Vitaly calls a positive integer <span class="tex-font-style-it">good</span>, if the decimal representation of this integer only contains digits <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. Vitaly calls a good number <span class="tex-font-style-it">excellent</span>, if the sum of its digits is a good number.</p><p>For example, let's say that Vitaly's favourite digits are <span class="tex-span">1</span> and <span class="tex-span">3</span>, then number <span class="tex-span">12</span> isn't good and numbers <span class="tex-span">13</span> or <span class="tex-span">311</span> are. Also, number <span class="tex-span">111</span> is excellent and number <span class="tex-span">11</span> isn't. </p><p>Now Vitaly is wondering, how many excellent numbers of length exactly <span class="tex-span"><i>n</i></span> are there. As this number can be rather large, he asks you to count the remainder after dividing it by <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p><p>A number's length is the number of digits in its decimal representation without leading zeroes.</p></div><div class="input-specification"><p>The first line contains three integers: <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>a</i> &lt; <i>b</i> ≤ 9, 1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>)</span>.</p></div><div class="output-specification"><p>Print a single integer — the answer to the problem modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains three integers: <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>a</i> &lt; <i>b</i> ≤ 9, 1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>)</span>.</p>

## Output

<p>Print a single integer — the answer to the problem modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
1 3 3

```




```input2
2 3 10

```




```output1
1

```




```output2
165

```


