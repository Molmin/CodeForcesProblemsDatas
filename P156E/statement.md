## Description

<div><p>Mrs. Hudson hasn't made her famous pancakes for quite a while and finally she decided to make them again. She has learned <span class="tex-span"><i>m</i></span> new recipes recently and she can't wait to try them. Those recipes are based on <span class="tex-span"><i>n</i></span> special spices. Mrs. Hudson has these spices in the kitchen lying in jars <span class="tex-font-style-bf">numbered</span> with integers from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i> - 1</span> (each spice lies in an individual jar). Each jar also has the <span class="tex-font-style-bf">price</span> of the corresponding spice inscribed — some integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>We know three values for the <span class="tex-span"><i>i</i></span>-th pancake recipe: <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>. Here <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> are integers, and <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> is the <span class="tex-font-style-underline">pattern</span> of some integer written in the numeral system with radix <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>. The pattern contains digits, Latin letters (to denote digits larger than nine) and question marks. Number <span class="tex-span"><i>x</i></span> in the <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>-base numeral system <span class="tex-font-style-underline">matches the pattern</span> <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>, if we can replace question marks in the pattern with digits and letters so that we obtain number <span class="tex-span"><i>x</i></span> (leading zeroes aren't taken into consideration when performing the comparison). More formally: each question mark should be replaced by exactly one digit or exactly one letter. If after we replace all question marks we get a number with leading zeroes, we can delete these zeroes. For example, number <span class="tex-font-style-tt">40A9875</span> in the <span class="tex-span">11</span>-base numeral system matches the pattern "<span class="tex-font-style-tt">??4??987?</span>", and number <span class="tex-font-style-tt">4A9875</span> does not.</p><p>To make the pancakes by the <span class="tex-span"><i>i</i></span>-th recipe, Mrs. Hudson should take all jars with <span class="tex-font-style-bf">numbers</span> whose representation in the <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>-base numeral system matches the pattern <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>. The <span class="tex-font-style-underline">control number</span> of the recipe (<span class="tex-span"><i>z</i><sub class="lower-index"><i>i</i></sub></span>) is defined as the sum of number <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and the product of <span class="tex-font-style-bf">prices</span> of all taken jars. More formally: <img align="middle" class="tex-formula" src="file://GBaUJ4ou.png" style="max-width: 100.0%;max-height: 100.0%;"> (where <span class="tex-span"><i>j</i></span> is all such numbers whose representation in the <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>-base numeral system matches the pattern <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>).</p><p>Mrs. Hudson isn't as interested in the control numbers as she is in their minimum prime divisors. Your task is: for each recipe <span class="tex-span"><i>i</i></span> find the minimum prime divisor of number <span class="tex-span"><i>z</i><sub class="lower-index"><i>i</i></sub></span>. If this divisor exceeds <span class="tex-span">100</span>, then you do not have to find it, print -1.</p></div><div class="input-specification"><p>The first line contains the single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup></span>). The second line contains space-separated prices of the spices <span class="tex-span"><i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is an integer (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>).</p><p>The third line contains the single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">4</sup></span>) — the number of recipes Mrs. Hudson has learned. </p><p>Next <span class="tex-span"><i>m</i></span> lines describe the recipes, one per line. First you are given an integer <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>, written in the decimal numeral system (<span class="tex-span">2 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 16</span>). Then after a space follows the <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> pattern — a string from <span class="tex-span">1</span> to <span class="tex-span">30</span> in length, inclusive, consisting of digits from "<span class="tex-font-style-tt">0</span>" to "<span class="tex-font-style-tt">9</span>", letters from "<span class="tex-font-style-tt">A</span>" to "<span class="tex-font-style-tt">F</span>" and signs "<span class="tex-font-style-tt">?</span>". Letters from "<span class="tex-font-style-tt">A</span>" to "<span class="tex-font-style-tt">F</span>" should be considered as digits from <span class="tex-span">10</span> to <span class="tex-span">15</span> correspondingly. It is guaranteed that all digits of the pattern (including the digits that are represented by letters) are strictly less than <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>. Then after a space follows an integer <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, written in the decimal numeral system (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>).</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in С++, in is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span>, strings or the <span class="tex-font-style-tt">%I64d</span> specificator instead.</p></div><div class="output-specification"><p>For each recipe count by what minimum prime number the control number is divided and print this prime number on the single line. If this number turns out larger than <span class="tex-span">100</span>, print -1.</p></div>

## Input

<p>The first line contains the single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup></span>). The second line contains space-separated prices of the spices <span class="tex-span"><i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is an integer (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>).</p><p>The third line contains the single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">4</sup></span>) — the number of recipes Mrs. Hudson has learned. </p><p>Next <span class="tex-span"><i>m</i></span> lines describe the recipes, one per line. First you are given an integer <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>, written in the decimal numeral system (<span class="tex-span">2 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 16</span>). Then after a space follows the <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> pattern — a string from <span class="tex-span">1</span> to <span class="tex-span">30</span> in length, inclusive, consisting of digits from "<span class="tex-font-style-tt">0</span>" to "<span class="tex-font-style-tt">9</span>", letters from "<span class="tex-font-style-tt">A</span>" to "<span class="tex-font-style-tt">F</span>" and signs "<span class="tex-font-style-tt">?</span>". Letters from "<span class="tex-font-style-tt">A</span>" to "<span class="tex-font-style-tt">F</span>" should be considered as digits from <span class="tex-span">10</span> to <span class="tex-span">15</span> correspondingly. It is guaranteed that all digits of the pattern (including the digits that are represented by letters) are strictly less than <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>. Then after a space follows an integer <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, written in the decimal numeral system (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>).</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in С++, in is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span>, strings or the <span class="tex-font-style-tt">%I64d</span> specificator instead.</p>

## Output

<p>For each recipe count by what minimum prime number the control number is divided and print this prime number on the single line. If this number turns out larger than <span class="tex-span">100</span>, print -1.</p>





```input1
1
1
1
2 ? 1

```




```input2
4
2 3 5 7
4
2 ?0 11
2 ?1 13
2 0? 17
2 1? 19

```




```input3
1
1000000000000000000
1
16 ?????????????? 1

```




```output1
2

```




```output2
3
2
23
2

```




```output3
-1

```



## Note

<p>In the first test any one-digit number in the binary system matches. The jar is only one and its price is equal to <span class="tex-span">1</span>, the number <span class="tex-span"><i>c</i></span> is also equal to <span class="tex-span">1</span>, the control number equals <span class="tex-span">2</span>. The minimal prime divisor of <span class="tex-span">2</span> is <span class="tex-span">2</span>.</p><p>In the second test there are <span class="tex-span">4</span> jars with numbers from <span class="tex-span">0</span> to <span class="tex-span">3</span>, and the prices are equal <span class="tex-span">2</span>, <span class="tex-span">3</span>, <span class="tex-span">5</span> and <span class="tex-span">7</span> correspondingly — the first four prime numbers. In all recipes numbers should be two-digit. In the first recipe the second digit always is <span class="tex-span">0</span>, in the second recipe the second digit always is <span class="tex-span">1</span>, in the third recipe the first digit must be <span class="tex-span">0</span>, in the fourth recipe the first digit always is <span class="tex-span">1</span>. Consequently, the control numbers ​​are as follows: in the first recipe <span class="tex-span">2 × 5 + 11 = 21</span> (the minimum prime divisor is <span class="tex-span">3</span>), in the second recipe <span class="tex-span">3 × 7 + 13 = 44</span> (the minimum prime divisor is <span class="tex-span">2</span>), in the third recipe <span class="tex-span">2 × 3 + 17 = 23</span> (the minimum prime divisor is <span class="tex-span">23</span>) and, finally, in the fourth recipe <span class="tex-span">5 × 7 + 19 = 54</span> (the minimum prime divisor is <span class="tex-span">2</span>).</p><p>In the third test, the number should consist of fourteen digits and be recorded in a sixteen-base numeral system. Number <span class="tex-span">0</span> (the number of the single bottles) matches, the control number will be equal to <span class="tex-span">10<sup class="upper-index">18</sup> + 1</span>. The minimum prime divisor of this number is equal to <span class="tex-span">101</span> and you should print -1.</p>
