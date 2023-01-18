## Description

<div><p>Vasily exited from a store and now he wants to recheck the total price of all purchases in his bill. The bill is a string in which the names of the purchases and their prices are printed in a row without any spaces. Check has the format "<span class="tex-font-style-tt"><span class="tex-span"><i>name</i><sub class="lower-index">1</sub><i>price</i><sub class="lower-index">1</sub><i>name</i><sub class="lower-index">2</sub><i>price</i><sub class="lower-index">2</sub>...<i>name</i><sub class="lower-index"><i>n</i></sub><i>price</i><sub class="lower-index"><i>n</i></sub></span></span>", where <span class="tex-span"><i>name</i><sub class="lower-index"><i>i</i></sub></span> (name of the <span class="tex-span"><i>i</i></span>-th purchase) is a non-empty string of length not more than <span class="tex-span">10</span>, consisting of lowercase English letters, and <span class="tex-span"><i>price</i><sub class="lower-index"><i>i</i></sub></span> (the price of the <span class="tex-span"><i>i</i></span>-th purchase) is a non-empty string, consisting of digits and dots (decimal points). It is possible that purchases with equal names have different prices.</p><p>The price of each purchase is written in the following format. If the price is an integer number of dollars then cents are not written.</p><p>Otherwise, after the number of dollars a dot (decimal point) is written followed by cents <span class="tex-font-style-bf">in a two-digit format</span> (if number of cents is between <span class="tex-span">1</span> and <span class="tex-span">9</span> inclusively, there is a leading zero).</p><p>Also, every three digits (from less significant to the most) in dollars are separated by dot (decimal point). No extra leading zeroes are allowed. The price always starts with a digit and ends with a digit.</p><p>For example:</p><ul> <li> "<span class="tex-font-style-tt">234</span>", "<span class="tex-font-style-tt">1.544</span>", "<span class="tex-font-style-tt">149.431.10</span>", "<span class="tex-font-style-tt">0.99</span>" and "<span class="tex-font-style-tt">123.05</span>" are valid prices, </li><li> "<span class="tex-font-style-tt">.333</span>", "<span class="tex-font-style-tt">3.33.11</span>", "<span class="tex-font-style-tt">12.00</span>", "<span class="tex-font-style-tt">.33</span>", "<span class="tex-font-style-tt">0.1234</span>" and "<span class="tex-font-style-tt">1.2</span>" are not valid. </li></ul><p>Write a program that will find the total price of all purchases in the given bill.</p></div><div class="input-specification"><p>The only line of the input contains a non-empty string <span class="tex-span"><i>s</i></span> with length not greater than <span class="tex-span">1000</span>&nbsp;— the content of the bill.</p><p>It is guaranteed that the bill meets the format described above. It is guaranteed that each price in the bill is not less than one cent and not greater than <span class="tex-span">10<sup class="upper-index">6</sup></span> dollars.</p></div><div class="output-specification"><p>Print the total price <span class="tex-font-style-bf">exactly in the same format</span> as prices given in the input.</p></div>

## Input

<p>The only line of the input contains a non-empty string <span class="tex-span"><i>s</i></span> with length not greater than <span class="tex-span">1000</span>&nbsp;— the content of the bill.</p><p>It is guaranteed that the bill meets the format described above. It is guaranteed that each price in the bill is not less than one cent and not greater than <span class="tex-span">10<sup class="upper-index">6</sup></span> dollars.</p>

## Output

<p>Print the total price <span class="tex-font-style-bf">exactly in the same format</span> as prices given in the input.</p>





```input1
chipsy48.32televizor12.390

```




```input2
a1b2c3.38

```




```input3
aa0.01t0.03

```




```output1
12.438.32

```




```output2
6.38

```




```output3
0.04

```


