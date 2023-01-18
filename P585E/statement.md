## Description

<div><p>Vitalik the philatelist has a birthday today!</p><p>As he is a regular customer in a stamp store called 'Robin Bobin', the store management decided to make him a gift.</p><p>Vitalik wants to buy one stamp and the store will give him a non-empty set of the remaining stamps, such that the greatest common divisor (GCD) of the price of the stamps they give to him is more than one. If the GCD of prices of the purchased stamp and prices of present stamps set will be equal to <span class="tex-span">1</span>, then Vitalik will leave the store completely happy.</p><p>The store management asks you to count the number of different situations in which Vitalik will leave the store completely happy. Since the required number of situations can be very large, you need to find the remainder of this number modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>. The situations are different if the stamps purchased by Vitalik are different, or if one of the present sets contains a stamp that the other present does not contain.</p></div><div class="input-specification"><p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>) — the number of distinct stamps, available for sale in the 'Robin Bobin' store. </p><p>The second line contains a sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">2 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the price of the <span class="tex-span"><i>i</i></span>-th stamp.</p></div><div class="output-specification"><p>Print a single integer — the remainder of the sought number of situations modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>) — the number of distinct stamps, available for sale in the 'Robin Bobin' store. </p><p>The second line contains a sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">2 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the price of the <span class="tex-span"><i>i</i></span>-th stamp.</p>

## Output

<p>Print a single integer — the remainder of the sought number of situations modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
3
2 3 2

```




```input2
2
9 6

```




```output1
5

```




```output2
0

```



## Note

<p>In the first sample the following situations are possible: </p><ul> <li> Vitalik buys the 1-st stamp, the store gives him the 2-nd stamp as a present; </li><li> Vitalik buys the 3-rd stamp, the store gives him the 2-nd stamp as a present; </li><li> Vitalik buys the 2-nd stamp, the store gives him the 1-st stamp as a present; </li><li> Vitalik buys the 2-nd stamp, the store gives him the 3-rd stamp as a present; </li><li> Vitalik buys the 2-nd stamp, the store gives him the 1-st and 3-rd stamps as a present. </li></ul>
