## Description

<div><p>In a far away kingdom lived the King, the Prince, the Shoemaker, the Dressmaker and many other citizens. They lived happily until great trouble came into the Kingdom. The ACMers settled there.</p><p>Most damage those strange creatures inflicted upon the kingdom was that they loved high precision numbers. As a result, the Kingdom healers had already had three appointments with the merchants who were asked to sell, say, exactly <span class="tex-span">0.273549107</span> beer barrels. To deal with the problem somehow, the King issued an order obliging rounding up all numbers to the closest integer to simplify calculations. Specifically, the order went like this:</p><ul><li> If a number's integer part does not end with digit <span class="tex-span">9</span> and its fractional part is strictly less than <span class="tex-span">0.5</span>, then the rounded up number coincides with the number’s integer part. </li><li> If a number's integer part does not end with digit <span class="tex-span">9</span> and its fractional part is not less than <span class="tex-span">0.5</span>, the rounded up number is obtained if we add <span class="tex-span">1</span> to the last digit of the number’s integer part.</li><li> If the number’s integer part ends with digit <span class="tex-span">9</span>, to round up the numbers one should go to Vasilisa the Wise. In the whole Kingdom she is the only one who can perform the tricky operation of carrying into the next position. </li></ul><p>Merchants found the algorithm very sophisticated and they asked you (the ACMers) to help them. Can you write a program that would perform the rounding according to the King’s order?</p></div><div class="input-specification"><p>The first line contains a single number to round up — the integer part (a non-empty set of decimal digits that do not start with <span class="tex-span">0</span> — with the exception of a case when the set consists of a single digit — in this case 0 can go first), then follows character «<span class="tex-font-style-tt">.</span>» (a dot), and then follows the fractional part (any non-empty set of decimal digits). The number's length does not exceed <span class="tex-span">1000</span> characters, including the dot. There are no other characters in the input data.</p></div><div class="output-specification"><p>If the last number of the integer part is not equal to <span class="tex-span">9</span>, print the rounded-up number without leading zeroes. Otherwise, print the message "<span class="tex-font-style-tt">GOTO Vasilisa.</span>" (without the quotes).</p></div>

## Input

<p>The first line contains a single number to round up — the integer part (a non-empty set of decimal digits that do not start with <span class="tex-span">0</span> — with the exception of a case when the set consists of a single digit — in this case 0 can go first), then follows character «<span class="tex-font-style-tt">.</span>» (a dot), and then follows the fractional part (any non-empty set of decimal digits). The number's length does not exceed <span class="tex-span">1000</span> characters, including the dot. There are no other characters in the input data.</p>

## Output

<p>If the last number of the integer part is not equal to <span class="tex-span">9</span>, print the rounded-up number without leading zeroes. Otherwise, print the message "<span class="tex-font-style-tt">GOTO Vasilisa.</span>" (without the quotes).</p>





```input1
0.0

```




```input2
1.49

```




```input3
1.50

```




```input4
2.71828182845904523536

```




```input5
3.14159265358979323846

```




```input6
12345678901234567890.1

```




```input7
123456789123456789.999

```




```output1
0
```




```output2
1
```




```output3
2
```




```output4
3
```




```output5
3
```




```output6
12345678901234567890
```




```output7
GOTO Vasilisa.
```


