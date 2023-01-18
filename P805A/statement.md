## Description

<div><p>Tavak and Seyyed are good friends. Seyyed is very funny and he told Tavak to solve the following problem instead of <span class="tex-font-style-it">longest-path</span>.</p><p>You are given <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span>. For all integers from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span>, inclusive, we wrote down all of their integer divisors except <span class="tex-span">1</span>. Find the integer that we wrote down the maximum number of times.</p><p>Solve the problem to show that it's not a <span class="tex-font-style-it">NP</span> problem.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">2 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print single integer, the integer that appears maximum number of times in the divisors. </p><p>If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">2 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print single integer, the integer that appears maximum number of times in the divisors. </p><p>If there are multiple answers, print any of them.</p>





```input1
19 29

```




```input2
3 6

```




```output1
2

```




```output2
3

```



## Note

<p>Definition of a divisor: <a href="https://www.mathsisfun.com/definitions/divisor-of-an-integer-.html">https://www.mathsisfun.com/definitions/divisor-of-an-integer-.html</a></p><p>The first example: from <span class="tex-span">19</span> to <span class="tex-span">29</span> these numbers are divisible by <span class="tex-span">2</span>: <span class="tex-span">{20, 22, 24, 26, 28}</span>.</p><p>The second example: from <span class="tex-span">3</span> to <span class="tex-span">6</span> these numbers are divisible by <span class="tex-span">3</span>: <span class="tex-span">{3, 6}</span>.</p>
