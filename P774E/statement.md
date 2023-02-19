## Description

<div><p>Stepan has a very big positive integer.</p><p>Let's consider all cyclic shifts of Stepan's integer (if we look at his integer like at a string) which are also integers (i.e. they <span class="tex-font-style-bf">do not have</span> leading zeros). Let's call such shifts as <span class="tex-font-style-it">good shifts</span>. For example, for the integer <span class="tex-span">10203</span> the good shifts are the integer itself <span class="tex-span">10203</span> and integers <span class="tex-span">20310</span> and <span class="tex-span">31020</span>.</p><p>Stepan wants to know the minimum remainder of the division by the given number <span class="tex-span"><i>m</i></span> among all good shifts. Your task is to determine the minimum remainder of the division by <span class="tex-span"><i>m</i></span>.</p></div><div class="input-specification"><p>The first line contains the integer which Stepan has. The length of Stepan's integer is between <span class="tex-span">2</span> and <span class="tex-span">200 000</span> digits, inclusive. It is guaranteed that Stepan's integer does not contain leading zeros.</p><p>The second line contains the integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>m</i> ≤ 10<sup class="upper-index">8</sup></span>) — the number by which Stepan divides good shifts of his integer.</p></div><div class="output-specification"><p>Print the minimum remainder which Stepan can get if he divides all good shifts of his integer by the given number <span class="tex-span"><i>m</i></span>.</p></div>

## Input

<p>The first line contains the integer which Stepan has. The length of Stepan's integer is between <span class="tex-span">2</span> and <span class="tex-span">200 000</span> digits, inclusive. It is guaranteed that Stepan's integer does not contain leading zeros.</p><p>The second line contains the integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>m</i> ≤ 10<sup class="upper-index">8</sup></span>) — the number by which Stepan divides good shifts of his integer.</p>

## Output

<p>Print the minimum remainder which Stepan can get if he divides all good shifts of his integer by the given number <span class="tex-span"><i>m</i></span>.</p>





```input1
521
3

```




```input2
1001
5

```




```input3
5678901234567890123456789
10000

```




```output1
2

```




```output2
0

```




```output3
123

```



## Note

<p>In the first example all good shifts of the integer <span class="tex-span">521</span> (good shifts are equal to <span class="tex-span">521</span>, <span class="tex-span">215</span> and <span class="tex-span">152</span>) has same remainder <span class="tex-span">2</span> when dividing by <span class="tex-span">3</span>.</p><p>In the second example there are only two good shifts: the Stepan's integer itself and the shift by one position to the right. The integer itself is <span class="tex-span">1001</span> and the remainder after dividing it by <span class="tex-span">5</span> equals <span class="tex-span">1</span>. The shift by one position to the right equals to <span class="tex-span">1100</span> and the remainder after dividing it by <span class="tex-span">5</span> equals <span class="tex-span">0</span>, which is the minimum possible remainder.</p>
