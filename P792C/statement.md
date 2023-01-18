## Description

<div><p>A positive integer number <span class="tex-span"><i>n</i></span> is written on a blackboard. It consists of not more than <span class="tex-span">10<sup class="upper-index">5</sup></span> digits. You have to transform it into a <span class="tex-font-style-it">beautiful</span> number by erasing some of the digits, and you want to erase as few digits as possible.</p><p>The number is called beautiful if it consists of at least one digit, doesn't have leading zeroes and is a multiple of <span class="tex-span">3</span>. For example, <span class="tex-font-style-tt">0</span>, <span class="tex-font-style-tt">99</span>, <span class="tex-font-style-tt">10110</span> are beautiful numbers, and <span class="tex-font-style-tt">00</span>, <span class="tex-font-style-tt">03</span>, <span class="tex-font-style-tt">122</span> are not.</p><p>Write a program which for the given <span class="tex-span"><i>n</i></span> will find a beautiful number such that <span class="tex-span"><i>n</i></span> can be transformed into this number by erasing as few digits as possible. You can erase an arbitraty set of digits. For example, they don't have to go one after another in the number <span class="tex-span"><i>n</i></span>.</p><p>If it's impossible to obtain a beautiful number, print <span class="tex-font-style-tt">-1</span>. If there are multiple answers, print any of them.</p></div><div class="input-specification"><p>The first line of input contains <span class="tex-span"><i>n</i></span> — a positive integer number without leading zeroes (<span class="tex-span">1 ≤ <i>n</i> &lt; 10<sup class="upper-index">100000</sup></span>).</p></div><div class="output-specification"><p>Print one number — any beautiful number obtained by erasing as few as possible digits. If there is no answer, print <span class="tex-span"> - 1</span>.</p></div>

## Input

<p>The first line of input contains <span class="tex-span"><i>n</i></span> — a positive integer number without leading zeroes (<span class="tex-span">1 ≤ <i>n</i> &lt; 10<sup class="upper-index">100000</sup></span>).</p>

## Output

<p>Print one number — any beautiful number obtained by erasing as few as possible digits. If there is no answer, print <span class="tex-span"> - 1</span>.</p>





```input1
1033

```




```input2
10

```




```input3
11

```




```output1
33

```




```output2
0

```




```output3
-1

```



## Note

<p>In the first example it is enough to erase only the first digit to obtain a multiple of <span class="tex-span">3</span>. But if we erase the first digit, then we obtain a number with a leading zero. So the minimum number of digits to be erased is two.</p>
