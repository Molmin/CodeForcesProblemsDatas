## Description

<div><p>Polycarpus is an amateur businessman. Recently he was surprised to find out that the market for paper scissors is completely free! Without further ado, Polycarpus decided to start producing and selling such scissors.</p><p>Polycaprus calculated that the optimal celling price for such scissors would be <span class="tex-span"><i>p</i></span> bourles. However, he read somewhere that customers are attracted by prices that say something like "Special Offer! Super price 999 bourles!". So Polycarpus decided to lower the price a little if it leads to the desired effect.</p><p>Polycarpus agrees to lower the price by no more than <span class="tex-span"><i>d</i></span> bourles so that the number of nines at the end of the resulting price is maximum. If there are several ways to do it, he chooses the maximum possible price.</p><p>Note, Polycarpus counts only the <span class="tex-font-style-it">trailing</span> nines in a price.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>p</i> ≤ 10<sup class="upper-index">18</sup></span>; <span class="tex-span">0 ≤ <i>d</i> &lt; <i>p</i></span>) — the initial price of scissors and the maximum possible price reduction.</p><p>Please, do not use the %lld specifier to read or write 64-bit integers in С++. It is preferred to use cin, cout streams or the %I64d specifier.</p></div><div class="output-specification"><p>Print the required price — the maximum price that ends with the largest number of nines and that is less than <span class="tex-span"><i>p</i></span> by no more than <span class="tex-span"><i>d</i></span>.</p><p>The required number shouldn't have leading zeroes.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>p</i> ≤ 10<sup class="upper-index">18</sup></span>; <span class="tex-span">0 ≤ <i>d</i> &lt; <i>p</i></span>) — the initial price of scissors and the maximum possible price reduction.</p><p>Please, do not use the %lld specifier to read or write 64-bit integers in С++. It is preferred to use cin, cout streams or the %I64d specifier.</p>

## Output

<p>Print the required price — the maximum price that ends with the largest number of nines and that is less than <span class="tex-span"><i>p</i></span> by no more than <span class="tex-span"><i>d</i></span>.</p><p>The required number shouldn't have leading zeroes.</p>





```input1
1029 102

```




```input2
27191 17

```




```output1
999

```




```output2
27189

```


