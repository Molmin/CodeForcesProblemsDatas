## Description

<div><p>Duff is in love with lovely numbers! A positive integer <span class="tex-span"><i>x</i></span> is called <span class="tex-font-style-it">lovely</span> if and only if there is no such positive integer <span class="tex-span"><i>a</i> &gt; 1</span> such that <span class="tex-span"><i>a</i><sup class="upper-index">2</sup></span> is a divisor of <span class="tex-span"><i>x</i></span>.</p><center> <img class="tex-graphics" src="file://Z5eDV42f.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Malek has a number store! In his store, he has only divisors of positive integer <span class="tex-span"><i>n</i></span> (and he has all of them). As a birthday present, Malek wants to give her a <span class="tex-font-style-it">lovely</span> number from his store. He wants this number to be as big as possible.</p><p>Malek always had issues in math, so he asked for your help. Please tell him what is the biggest lovely number in his store.</p></div><div class="input-specification"><p>The first and only line of input contains one integer, <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">12</sup></span>).</p></div><div class="output-specification"><p>Print the answer in one line.</p></div>

## Input

<p>The first and only line of input contains one integer, <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">12</sup></span>).</p>

## Output

<p>Print the answer in one line.</p>





```input1
10

```




```input2
12

```




```output1
10

```




```output2
6

```



## Note

<p>In first sample case, there are numbers 1, 2, 5 and 10 in the shop. 10 isn't divisible by any perfect square, so 10 is <span class="tex-font-style-it">lovely</span>.</p><p>In second sample case, there are numbers 1, 2, 3, 4, 6 and 12 in the shop. 12 is divisible by <span class="tex-span">4 = 2<sup class="upper-index">2</sup></span>, so 12 is not <span class="tex-font-style-it">lovely</span>, while 6 is indeed <span class="tex-font-style-it">lovely</span>.</p>
