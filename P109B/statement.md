## Description

<div><p><span class="tex-font-style-underline">Petya loves lucky numbers. We all know that lucky numbers are the positive integers whose decimal representations contain only the lucky digits <span class="tex-font-style-bf">4</span> and <span class="tex-font-style-bf">7</span>. For example, numbers <span class="tex-font-style-bf">47</span>, <span class="tex-font-style-bf">744</span>, <span class="tex-font-style-bf">4</span> are lucky and <span class="tex-font-style-bf">5</span>, <span class="tex-font-style-bf">17</span>, <span class="tex-font-style-bf">467</span> are not.</span></p><p>Petya and his friend Vasya play an interesting game. Petya randomly chooses an integer <span class="tex-span"><i>p</i></span> from the interval <span class="tex-span">[<i>p</i><sub class="lower-index"><i>l</i></sub>, <i>p</i><sub class="lower-index"><i>r</i></sub>]</span> and Vasya chooses an integer <span class="tex-span"><i>v</i></span> from the interval <span class="tex-span">[<i>v</i><sub class="lower-index"><i>l</i></sub>, <i>v</i><sub class="lower-index"><i>r</i></sub>]</span> (also randomly). Both players choose their integers equiprobably. Find the probability that the interval <span class="tex-span">[<i>min</i>(<i>v</i>, <i>p</i>), <i>max</i>(<i>v</i>, <i>p</i>)]</span> contains exactly <span class="tex-span"><i>k</i></span> lucky numbers.</p></div><div class="input-specification"><p>The single line contains five integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>l</i></sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>r</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>l</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>r</i></sub></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>l</i></sub> ≤ <i>p</i><sub class="lower-index"><i>r</i></sub> ≤ 10<sup class="upper-index">9</sup>, 1 ≤ <i>v</i><sub class="lower-index"><i>l</i></sub> ≤ <i>v</i><sub class="lower-index"><i>r</i></sub> ≤ 10<sup class="upper-index">9</sup>, 1 ≤ <i>k</i> ≤ 1000</span>).</p></div><div class="output-specification"><p>On the single line print the result with an absolute error of no more than <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p></div>

## Input

<p>The single line contains five integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>l</i></sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>r</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>l</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>r</i></sub></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>l</i></sub> ≤ <i>p</i><sub class="lower-index"><i>r</i></sub> ≤ 10<sup class="upper-index">9</sup>, 1 ≤ <i>v</i><sub class="lower-index"><i>l</i></sub> ≤ <i>v</i><sub class="lower-index"><i>r</i></sub> ≤ 10<sup class="upper-index">9</sup>, 1 ≤ <i>k</i> ≤ 1000</span>).</p>

## Output

<p>On the single line print the result with an absolute error of no more than <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p>





```input1
1 10 1 10 2

```




```input2
5 6 8 10 1

```




```output1
0.320000000000

```




```output2
1.000000000000

```



## Note

<p>Consider that <span class="tex-span">[<i>a</i>, <i>b</i>]</span> denotes an interval of integers; this interval <span class="tex-font-style-bf">includes</span> the boundaries. That is, <img align="middle" class="tex-formula" src="file://fYhxZuG9.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>In first case there are <span class="tex-span">32</span> suitable pairs: <span class="tex-span">(1, 7), (1, 8), (1, 9), (1, 10), (2, 7), (2, 8), (2, 9), (2, 10), (3, 7), (3, 8), (3, 9), (3, 10), (4, 7), (4, 8), (4, 9), (4, 10), (7, 1), (7, 2), (7, 3), (7, 4), (8, 1), (8, 2), (8, 3), (8, 4), (9, 1), (9, 2), (9, 3), (9, 4), (10, 1), (10, 2), (10, 3), (10, 4)</span>. Total number of possible pairs is <span class="tex-span">10·10 = 100</span>, so answer is <span class="tex-span">32 / 100</span>.</p><p>In second case Petya always get number less than Vasya and the only lucky <span class="tex-span">7</span> is between this numbers, so there will be always <span class="tex-span">1</span> lucky number.</p>
