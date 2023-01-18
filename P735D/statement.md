## Description

<div><p>Mr. Funt now lives in a country with a very specific tax laws. The total income of mr. Funt during this year is equal to <span class="tex-span"><i>n</i></span> (<span class="tex-span"><i>n</i> ≥ 2</span>) burles and the amount of tax he has to pay is calculated as the maximum divisor of <span class="tex-span"><i>n</i></span> (not equal to <span class="tex-span"><i>n</i></span>, of course). For example, if <span class="tex-span"><i>n</i> = 6</span> then Funt has to pay <span class="tex-span">3</span> burles, while for <span class="tex-span"><i>n</i> = 25</span> he needs to pay <span class="tex-span">5</span> and if <span class="tex-span"><i>n</i> = 2</span> he pays only <span class="tex-span">1</span> burle.</p><p>As mr. Funt is a very opportunistic person he wants to cheat a bit. In particular, he wants to split the initial <span class="tex-span"><i>n</i></span> in several parts <span class="tex-span"><i>n</i><sub class="lower-index">1</sub> + <i>n</i><sub class="lower-index">2</sub> + ... + <i>n</i><sub class="lower-index"><i>k</i></sub> = <i>n</i></span> (here <span class="tex-span"><i>k</i></span> is arbitrary, even <span class="tex-span"><i>k</i> = 1</span> is allowed) and pay the taxes for each part separately. He can't make some part equal to <span class="tex-span">1</span> because it will reveal him. So, the condition <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub> ≥ 2</span> should hold for all <span class="tex-span"><i>i</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i></span>.</p><p>Ostap Bender wonders, how many money Funt has to pay (i.e. minimal) if he chooses and optimal way to split <span class="tex-span"><i>n</i></span> in parts.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">9</sup></span>)&nbsp;— the total year income of mr. Funt.</p></div><div class="output-specification"><p>Print one integer&nbsp;— minimum possible number of burles that mr. Funt has to pay as a tax.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">9</sup></span>)&nbsp;— the total year income of mr. Funt.</p>

## Output

<p>Print one integer&nbsp;— minimum possible number of burles that mr. Funt has to pay as a tax.</p>





```input1
4

```




```input2
27

```




```output1
2

```




```output2
3

```


