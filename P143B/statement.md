## Description

<div><p>For some time the program of rounding numbers that had been developed by the Codeforces participants during one of the previous rounds, helped the citizens of Far Far Away to convert numbers into a more easily readable format. However, as time went by, the economy of the Far Far Away developed and the scale of operations grew. So the King ordered to found the Bank of Far Far Away and very soon even the rounding didn't help to quickly determine even the order of the numbers involved in operations. Besides, rounding a number to an integer wasn't very convenient as a bank needed to operate with all numbers with accuracy of up to <span class="tex-span">0.01</span>, and not up to an integer.</p><p>The King issued yet another order: to introduce financial format to represent numbers denoting amounts of money. The formal rules of storing a number in the financial format are as follows: </p><ul> <li> A number contains the integer part and the fractional part. The two parts are separated with a character "<span class="tex-font-style-tt">.</span>" (decimal point). </li><li> To make digits in the integer part of a number easier to read, they are split into groups of three digits, starting from the least significant ones. The groups are separated with the character "<span class="tex-font-style-tt">,</span>" (comma). For example, if the integer part of a number equals 12345678, then it will be stored in the financial format as 12,345,678 </li><li> In the financial format a number's fractional part should contain exactly two digits. So, if the initial number (the number that is converted into the financial format) contains less than two digits in the fractional part (or contains no digits at all), it is complemented with zeros until its length equals 2. If the fractional part contains more than two digits, the extra digits are simply <span class="tex-font-style-bf">discarded</span> (they are not rounded: see sample tests). </li><li> When a number is stored in the financial format, the minus sign is not written. Instead, if the initial number had the minus sign, the result is written in round brackets. </li><li> Please keep in mind that the bank of Far Far Away operates using an exotic foreign currency — snakes ($), that's why right before the number in the financial format we should put the sign "<span class="tex-font-style-tt">$</span>". If the number should be written in the brackets, then the snake sign should also be inside the brackets. </li></ul><p>For example, by the above given rules number 2012 will be stored in the financial format as "<span class="tex-font-style-tt">$2,012.00</span>" and number -12345678.9 will be stored as "<span class="tex-font-style-tt">($12,345,678.90)</span>".</p><p>The merchants of Far Far Away visited you again and expressed much hope that you supply them with the program that can convert arbitrary numbers to the financial format. Can you help them?</p></div><div class="input-specification"><p>The input contains a number that needs to be converted into financial format. The number's notation length does not exceed <span class="tex-span">100</span> characters, including (possible) signs "<span class="tex-font-style-tt">-</span>" (minus) and "<span class="tex-font-style-tt">.</span>" (decimal point). The number's notation is correct, that is: </p><ul> <li> The number's notation only contains characters from the set {"<span class="tex-font-style-tt">0</span>" – "<span class="tex-font-style-tt">9</span>", "<span class="tex-font-style-tt">-</span>", "<span class="tex-font-style-tt">.</span>"}. </li><li> The decimal point (if it is present) is unique and is preceded and followed by a non-zero quantity on decimal digits </li><li> A number cannot start with digit <span class="tex-span">0</span>, except for a case when its whole integer part equals zero (in this case the integer parts is guaranteed to be a single zero: "<span class="tex-font-style-tt">0</span>"). </li><li> The minus sign (if it is present) is unique and stands in the very beginning of the number's notation </li><li> If a number is identically equal to <span class="tex-span">0</span> (that is, if it is written as, for example, "<span class="tex-font-style-tt">0</span>" or "<span class="tex-font-style-tt">0.000</span>"), than it is not preceded by the minus sign. </li><li> The input data contains no spaces. </li><li> The number's notation contains at least one decimal digit. </li></ul></div><div class="output-specification"><p>Print the number given in the input in the financial format by the rules described in the problem statement.</p></div>

## Input

<p>The input contains a number that needs to be converted into financial format. The number's notation length does not exceed <span class="tex-span">100</span> characters, including (possible) signs "<span class="tex-font-style-tt">-</span>" (minus) and "<span class="tex-font-style-tt">.</span>" (decimal point). The number's notation is correct, that is: </p><ul> <li> The number's notation only contains characters from the set {"<span class="tex-font-style-tt">0</span>" – "<span class="tex-font-style-tt">9</span>", "<span class="tex-font-style-tt">-</span>", "<span class="tex-font-style-tt">.</span>"}. </li><li> The decimal point (if it is present) is unique and is preceded and followed by a non-zero quantity on decimal digits </li><li> A number cannot start with digit <span class="tex-span">0</span>, except for a case when its whole integer part equals zero (in this case the integer parts is guaranteed to be a single zero: "<span class="tex-font-style-tt">0</span>"). </li><li> The minus sign (if it is present) is unique and stands in the very beginning of the number's notation </li><li> If a number is identically equal to <span class="tex-span">0</span> (that is, if it is written as, for example, "<span class="tex-font-style-tt">0</span>" or "<span class="tex-font-style-tt">0.000</span>"), than it is not preceded by the minus sign. </li><li> The input data contains no spaces. </li><li> The number's notation contains at least one decimal digit. </li></ul>

## Output

<p>Print the number given in the input in the financial format by the rules described in the problem statement.</p>





```input1
2012

```




```input2
0.000

```




```input3
-0.00987654321

```




```input4
-12345678.9

```




```output1
$2,012.00
```




```output2
$0.00
```




```output3
($0.00)
```




```output4
($12,345,678.90)
```



## Note

<p>Pay attention to the second and third sample tests. They show that the sign of a number in the financial format (and consequently, the presence or absence of brackets) is determined solely by the sign of the initial number. It does not depend on the sign of the number you got after translating the number to the financial format.</p>
