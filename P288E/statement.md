## Description

<div><p><span class="tex-font-style-underline">Everybody knows that lucky numbers are positive integers that contain only lucky digits 4 and 7 in their decimal representation. For example, numbers 47, 744, 4 are lucky and 5, 17, 467 are not.</span></p><p>Polo the Penguin have two positive integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> <span class="tex-span">(<i>l</i> &lt; <i>r</i>)</span>, both of them are lucky numbers. Moreover, their lengths (that is, the number of digits in the decimal representation without the leading zeroes) are equal to each other.</p><p>Let's assume that <span class="tex-span"><i>n</i></span> is the number of distinct lucky numbers, each of them cannot be greater than <span class="tex-span"><i>r</i></span> or less than <span class="tex-span"><i>l</i></span>, and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the <span class="tex-span"><i>i</i></span>-th (in increasing order) number of them. Find <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>·<i>a</i><sub class="lower-index">2</sub> + <i>a</i><sub class="lower-index">2</sub>·<i>a</i><sub class="lower-index">3</sub> + ... + <i>a</i><sub class="lower-index"><i>n</i> - 1</sub>·<i>a</i><sub class="lower-index"><i>n</i></sub></span>. As the answer can be rather large, print the remainder after dividing it by <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div><div class="input-specification"><p>The first line contains a positive integer <span class="tex-span"><i>l</i></span>, and the second line contains a positive integer <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> &lt; <i>r</i> ≤ 10<sup class="upper-index">100000</sup></span>). The numbers are given without any leading zeroes.</p><p>It is guaranteed that the lengths of the given numbers are equal to each other and that both of them are lucky numbers.</p></div><div class="output-specification"><p>In the single line print a single integer — the answer to the problem modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div>

## Input

<p>The first line contains a positive integer <span class="tex-span"><i>l</i></span>, and the second line contains a positive integer <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> &lt; <i>r</i> ≤ 10<sup class="upper-index">100000</sup></span>). The numbers are given without any leading zeroes.</p><p>It is guaranteed that the lengths of the given numbers are equal to each other and that both of them are lucky numbers.</p>

## Output

<p>In the single line print a single integer — the answer to the problem modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p>





```input1
4
7

```




```input2
474
777

```




```output1
28

```




```output2
2316330

```


