## Description

<div><p>Dima loves representing an odd number as the sum of multiple primes, and Lisa loves it when there are at most three primes. Help them to represent the given number as the sum of at most than three primes.</p><p>More formally, you are given an <span class="tex-font-style-bf">odd</span> numer <span class="tex-span"><i>n</i></span>. Find a set of numbers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>k</i></span>), such that</p><ol><li> <span class="tex-span">1 ≤ <i>k</i> ≤ 3</span></li><li> <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is a prime</li><li> <img align="middle" class="tex-formula" src="file://xFc3TYr3.png" style="max-width: 100.0%;max-height: 100.0%;"></li></ol><p>The numbers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> do not necessarily have to be distinct. It is guaranteed that at least one possible solution exists.</p></div><div class="input-specification"><p>The single line contains an odd number <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> &lt; 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>In the first line print <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ 3)</span>, showing how many numbers are in the representation you found.</p><p>In the second line print numbers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> in any order. If there are multiple possible solutions, you can print any of them.</p></div>

## Input

<p>The single line contains an odd number <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> &lt; 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>In the first line print <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ 3)</span>, showing how many numbers are in the representation you found.</p><p>In the second line print numbers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> in any order. If there are multiple possible solutions, you can print any of them.</p>





```input1
27

```




```output1
3
5 11 11

```



## Note

<p>A prime is an integer strictly larger than one that is divisible only by one and by itself.</p>
