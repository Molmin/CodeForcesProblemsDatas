## Description

<div><p>Alexander is learning how to convert numbers from the decimal system to any other, however, he doesn't know English letters, so he writes any number only as a decimal number, it means that instead of the letter <span class="tex-span"><i>A</i></span> he will write the number <span class="tex-span">10</span>. Thus, by converting the number <span class="tex-span">475</span> from decimal to hexadecimal system, he gets <span class="tex-span">11311</span> (<span class="tex-span">475 = 1·16<sup class="upper-index">2</sup> + 13·16<sup class="upper-index">1</sup> + 11·16<sup class="upper-index">0</sup></span>). Alexander lived calmly until he tried to convert the number back to the decimal number system.</p><p>Alexander remembers that he worked with little numbers so he asks to find the minimum decimal number so that by converting it to the system with the base <span class="tex-span"><i>n</i></span> he will get the number <span class="tex-span"><i>k</i></span>.</p></div><div class="input-specification"><p>The first line contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>). The second line contains the integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> &lt; 10<sup class="upper-index">60</sup></span>), it is guaranteed that the number <span class="tex-span"><i>k</i></span> contains no more than <span class="tex-span">60</span> symbols. All digits in the second line are strictly less than <span class="tex-span"><i>n</i></span>.</p><p>Alexander guarantees that the answer exists and does not exceed <span class="tex-span">10<sup class="upper-index">18</sup></span>.</p><p>The number <span class="tex-span"><i>k</i></span> doesn't contain leading zeros.</p></div><div class="output-specification"><p>Print the number <span class="tex-span"><i>x</i></span> (<span class="tex-span">0 ≤ <i>x</i> ≤ 10<sup class="upper-index">18</sup></span>)&nbsp;— the answer to the problem.</p></div>

## Input

<p>The first line contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>). The second line contains the integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> &lt; 10<sup class="upper-index">60</sup></span>), it is guaranteed that the number <span class="tex-span"><i>k</i></span> contains no more than <span class="tex-span">60</span> symbols. All digits in the second line are strictly less than <span class="tex-span"><i>n</i></span>.</p><p>Alexander guarantees that the answer exists and does not exceed <span class="tex-span">10<sup class="upper-index">18</sup></span>.</p><p>The number <span class="tex-span"><i>k</i></span> doesn't contain leading zeros.</p>

## Output

<p>Print the number <span class="tex-span"><i>x</i></span> (<span class="tex-span">0 ≤ <i>x</i> ≤ 10<sup class="upper-index">18</sup></span>)&nbsp;— the answer to the problem.</p>





```input1
13
12

```




```input2
16
11311

```




```input3
20
999

```




```input4
17
2016

```




```output1
12
```




```output2
475
```




```output3
3789
```




```output4
594
```



## Note

<p>In the first example <span class="tex-span">12</span> could be obtained by converting two numbers to the system with base <span class="tex-span">13</span>: <span class="tex-span">12 = 12·13<sup class="upper-index">0</sup></span> or <span class="tex-span">15 = 1·13<sup class="upper-index">1</sup> + 2·13<sup class="upper-index">0</sup></span>.</p>
