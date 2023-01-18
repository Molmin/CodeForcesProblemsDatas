## Description

<div><p>Since Grisha behaved well last year, at New Year's Eve he was visited by Ded Moroz who brought an enormous bag of gifts with him! The bag contains <span class="tex-span"><i>n</i></span> sweet candies from <span class="tex-font-style-it">the good ol' bakery</span>, each labeled from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> corresponding to its tastiness. No two candies have the same tastiness.</p><p>The choice of candies has a direct effect on Grisha's happiness. One can assume that he should take the tastiest ones&nbsp;— but no, the holiday magic turns things upside down. It is the xor-sum of tastinesses that matters, not the ordinary sum!</p><p>A xor-sum of a sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span> is defined as the bitwise XOR of all its elements: <img align="middle" class="tex-formula" src="file://Dcm2N8ga.png" style="max-width: 100.0%;max-height: 100.0%;">, here <img align="middle" class="tex-formula" src="file://2Ct6cMut.png" style="max-width: 100.0%;max-height: 100.0%;"> denotes the bitwise XOR operation; more about bitwise XOR can be found <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">here.</a></p><p>Ded Moroz warned Grisha he has more houses to visit, so Grisha can take <span class="tex-font-style-bf">no more than <span class="tex-span"><i>k</i></span></span> candies from the bag. Help Grisha determine the largest xor-sum (largest xor-sum means maximum happiness!) he can obtain.</p></div><div class="input-specification"><p>The sole string contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup></span>).</p></div><div class="output-specification"><p>Output one number&nbsp;— the largest possible xor-sum.</p></div>

## Input

<p>The sole string contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup></span>).</p>

## Output

<p>Output one number&nbsp;— the largest possible xor-sum.</p>





```input1
4 3

```




```input2
6 6

```




```output1
7

```




```output2
7

```



## Note

<p>In the first sample case, one optimal answer is <span class="tex-span">1</span>, <span class="tex-span">2</span> and <span class="tex-span">4</span>, giving the xor-sum of <span class="tex-span">7</span>.</p><p>In the second sample case, one can, for example, take all six candies and obtain the xor-sum of <span class="tex-span">7</span>.</p>
