## Description

<div><p>Polycarp urgently needs a shovel! He comes to the shop and chooses an appropriate one. The shovel that Policarp chooses is sold for <span class="tex-span"><i>k</i></span> burles. Assume that there is an unlimited number of such shovels in the shop.</p><p>In his pocket Polycarp has an unlimited number of "10-burle coins" and exactly one coin of <span class="tex-span"><i>r</i></span> burles (<span class="tex-span">1 ≤ <i>r</i> ≤ 9</span>).</p><p>What is the minimum number of shovels Polycarp has to buy so that he can pay for the purchase without any change? It is obvious that he can pay for 10 shovels without any change (by paying the requied amount of 10-burle coins and not using the coin of <span class="tex-span"><i>r</i></span> burles). But perhaps he can buy fewer shovels and pay without any change. Note that Polycarp should buy at least one shovel.</p></div><div class="input-specification"><p>The single line of input contains two integers <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>r</i> ≤ 9</span>)&nbsp;— the price of one shovel and the denomination of the coin in Polycarp's pocket that is different from "10-burle coins". </p><p>Remember that he has an unlimited number of coins in the denomination of 10, that is, Polycarp has enough money to buy any number of shovels.</p></div><div class="output-specification"><p>Print the required minimum number of shovels Polycarp has to buy so that he can pay for them without any change. </p></div>

## Input

<p>The single line of input contains two integers <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>r</i> ≤ 9</span>)&nbsp;— the price of one shovel and the denomination of the coin in Polycarp's pocket that is different from "10-burle coins". </p><p>Remember that he has an unlimited number of coins in the denomination of 10, that is, Polycarp has enough money to buy any number of shovels.</p>

## Output

<p>Print the required minimum number of shovels Polycarp has to buy so that he can pay for them without any change. </p>





```input1
117 3

```




```input2
237 7

```




```input3
15 2

```




```output1
9

```




```output2
1

```




```output3
2

```



## Note

<p>In the first example Polycarp can buy 9 shovels and pay <span class="tex-span">9·117 = 1053</span> burles. Indeed, he can pay this sum by using 10-burle coins and one 3-burle coin. He can't buy fewer shovels without any change.</p><p>In the second example it is enough for Polycarp to buy one shovel.</p><p>In the third example Polycarp should buy two shovels and pay <span class="tex-span">2·15 = 30</span> burles. It is obvious that he can pay this sum without any change. </p>
