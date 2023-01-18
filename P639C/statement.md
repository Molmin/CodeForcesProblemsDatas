## Description

<div><p>Limak is a little polar bear. He doesn't have many toys and thus he often plays with polynomials.</p><p>He considers a polynomial <span class="tex-font-style-it">valid</span> if its degree is <span class="tex-span"><i>n</i></span> and its coefficients are integers not exceeding <span class="tex-span"><i>k</i></span> by the absolute value. More formally:</p><p>Let <span class="tex-span"><i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> denote the coefficients, so <img align="middle" class="tex-formula" src="file://XRMGz7u6.png" style="max-width: 100.0%;max-height: 100.0%;">. Then, a polynomial <span class="tex-span"><i>P</i>(<i>x</i>)</span> is valid if all the following conditions are satisfied:</p><ul> <li> <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is integer for every <span class="tex-span"><i>i</i></span>; </li><li> <span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ <i>k</i></span> for every <span class="tex-span"><i>i</i></span>; </li><li> <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub> ≠ 0</span>. </li></ul><p>Limak has recently got a valid polynomial <span class="tex-span"><i>P</i></span> with coefficients <span class="tex-span"><i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. He noticed that <span class="tex-span"><i>P</i>(2) ≠ 0</span> and he wants to change it. He is going to change one coefficient to get a <span class="tex-font-style-bf">valid</span> polynomial <span class="tex-span"><i>Q</i></span> of degree <span class="tex-span"><i>n</i></span> that <span class="tex-span"><i>Q</i>(2) = 0</span>. Count the number of ways to do so. You should count two ways as a distinct if coefficients of target polynoms differ.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000, 1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the degree of the polynomial and the limit for absolute values of coefficients.</p><p>The second line contains <span class="tex-span"><i>n</i> + 1</span> integers <span class="tex-span"><i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ <i>k</i>, <i>a</i><sub class="lower-index"><i>n</i></sub> ≠ 0</span>)&nbsp;— describing a <span class="tex-font-style-bf">valid</span> polynomial <img align="middle" class="tex-formula" src="file://gG6p56B0.png" style="max-width: 100.0%;max-height: 100.0%;">. It's guaranteed that <span class="tex-span"><i>P</i>(2) ≠ 0</span>.</p></div><div class="output-specification"><p>Print the number of ways to change one coefficient to get a valid polynomial <span class="tex-span"><i>Q</i></span> that <span class="tex-span"><i>Q</i>(2) = 0</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000, 1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the degree of the polynomial and the limit for absolute values of coefficients.</p><p>The second line contains <span class="tex-span"><i>n</i> + 1</span> integers <span class="tex-span"><i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ <i>k</i>, <i>a</i><sub class="lower-index"><i>n</i></sub> ≠ 0</span>)&nbsp;— describing a <span class="tex-font-style-bf">valid</span> polynomial <img align="middle" class="tex-formula" src="file://gG6p56B0.png" style="max-width: 100.0%;max-height: 100.0%;">. It's guaranteed that <span class="tex-span"><i>P</i>(2) ≠ 0</span>.</p>

## Output

<p>Print the number of ways to change one coefficient to get a valid polynomial <span class="tex-span"><i>Q</i></span> that <span class="tex-span"><i>Q</i>(2) = 0</span>.</p>





```input1
3 1000000000
10 -9 -3 5

```




```input2
3 12
10 -9 -3 5

```




```input3
2 20
14 -7 19

```




```output1
3

```




```output2
2

```




```output3
0

```



## Note

<p>In the first sample, we are given a polynomial <span class="tex-span"><i>P</i>(<i>x</i>) = 10 - 9<i>x</i> - 3<i>x</i><sup class="upper-index">2</sup> + 5<i>x</i><sup class="upper-index">3</sup></span>.</p><p>Limak can change one coefficient in three ways:</p><ol> <li> He can set <span class="tex-span"><i>a</i><sub class="lower-index">0</sub> =  - 10</span>. Then he would get <span class="tex-span"><i>Q</i>(<i>x</i>) =  - 10 - 9<i>x</i> - 3<i>x</i><sup class="upper-index">2</sup> + 5<i>x</i><sup class="upper-index">3</sup></span> and indeed <span class="tex-span"><i>Q</i>(2) =  - 10 - 18 - 12 + 40 = 0</span>. </li><li> Or he can set <span class="tex-span"><i>a</i><sub class="lower-index">2</sub> =  - 8</span>. Then <span class="tex-span"><i>Q</i>(<i>x</i>) = 10 - 9<i>x</i> - 8<i>x</i><sup class="upper-index">2</sup> + 5<i>x</i><sup class="upper-index">3</sup></span> and indeed <span class="tex-span"><i>Q</i>(2) = 10 - 18 - 32 + 40 = 0</span>. </li><li> Or he can set <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> =  - 19</span>. Then <span class="tex-span"><i>Q</i>(<i>x</i>) = 10 - 19<i>x</i> - 3<i>x</i><sup class="upper-index">2</sup> + 5<i>x</i><sup class="upper-index">3</sup></span> and indeed <span class="tex-span"><i>Q</i>(2) = 10 - 38 - 12 + 40 = 0</span>. </li></ol><p>In the second sample, we are given the same polynomial. This time though, <span class="tex-span"><i>k</i></span> is equal to <span class="tex-span">12</span> instead of <span class="tex-span">10<sup class="upper-index">9</sup></span>. Two first of ways listed above are still valid but in the third way we would get <span class="tex-span">|<i>a</i><sub class="lower-index">1</sub>| &gt; <i>k</i></span> what is not allowed. Thus, the answer is <span class="tex-span">2</span> this time.</p>
