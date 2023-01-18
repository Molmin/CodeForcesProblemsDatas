## Description

<div><p>In a far away kingdom young pages help to set the table for the King. As they are terribly mischievous, one needs to keep an eye on the control whether they have set everything correctly. This time the royal chef Gerasim had the impression that the pages have played a prank again: they had poured the juice from one cup to another. Now Gerasim wants to check his hypothesis. The good thing is that chef Gerasim always pour the same number of milliliters of juice to all cups in the royal kitchen. Having thoroughly measured the juice in each cup, Gerasim asked you to write a program that will determine from which cup juice was poured to which one; otherwise, the program should determine that this time the pages set the table diligently.</p><p>To simplify your task we shall consider the cups to be bottomless so that the juice never overfills a cup and pours out, however much it can be. Besides, by some strange reason in a far away kingdom one can only pour to a cup or from one cup to another an integer number of milliliters of juice.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> — the number of cups on the royal table (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>). Next <span class="tex-span"><i>n</i></span> lines contain volumes of juice in each cup — non-negative integers, not exceeding <span class="tex-span">10<sup class="upper-index">4</sup></span>.</p></div><div class="output-specification"><p>If the pages didn't pour the juice, print "<span class="tex-font-style-tt">Exemplary pages.</span>" (without the quotes). If you can determine the volume of juice poured during exactly one juice pouring, print "<span class="tex-font-style-tt"><span class="tex-span"><i>v</i></span> ml. from cup #<span class="tex-span"><i>a</i></span> to cup #<span class="tex-span"><i>b</i></span>.</span>" (without the quotes), where <span class="tex-span"><i>v</i></span> represents the volume of poured juice, <span class="tex-span"><i>a</i></span> represents the number of the cup from which the juice was poured (the cups are numbered with consecutive positive integers starting from one in the order in which the cups are described in the input data), <span class="tex-span"><i>b</i></span> represents the number of the cup into which the juice was poured. Finally, if the given juice's volumes cannot be obtained using no more than one pouring (for example, the pages poured the juice from one cup to another more than once or the royal kitchen maids poured the juice into the cups incorrectly), print "<span class="tex-font-style-tt">Unrecoverable configuration.</span>" (without the quotes).</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> — the number of cups on the royal table (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>). Next <span class="tex-span"><i>n</i></span> lines contain volumes of juice in each cup — non-negative integers, not exceeding <span class="tex-span">10<sup class="upper-index">4</sup></span>.</p>

## Output

<p>If the pages didn't pour the juice, print "<span class="tex-font-style-tt">Exemplary pages.</span>" (without the quotes). If you can determine the volume of juice poured during exactly one juice pouring, print "<span class="tex-font-style-tt"><span class="tex-span"><i>v</i></span> ml. from cup #<span class="tex-span"><i>a</i></span> to cup #<span class="tex-span"><i>b</i></span>.</span>" (without the quotes), where <span class="tex-span"><i>v</i></span> represents the volume of poured juice, <span class="tex-span"><i>a</i></span> represents the number of the cup from which the juice was poured (the cups are numbered with consecutive positive integers starting from one in the order in which the cups are described in the input data), <span class="tex-span"><i>b</i></span> represents the number of the cup into which the juice was poured. Finally, if the given juice's volumes cannot be obtained using no more than one pouring (for example, the pages poured the juice from one cup to another more than once or the royal kitchen maids poured the juice into the cups incorrectly), print "<span class="tex-font-style-tt">Unrecoverable configuration.</span>" (without the quotes).</p>





```input1
5
270
250
250
230
250

```




```input2
5
250
250
250
250
250

```




```input3
5
270
250
249
230
250

```




```output1
20 ml. from cup #4 to cup #1.

```




```output2
Exemplary pages.

```




```output3
Unrecoverable configuration.

```


