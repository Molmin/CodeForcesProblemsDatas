## Description

<div><p>Not long ago Billy came across such a problem, where there were given three natural numbers <span class="tex-span"><i>A</i></span>, <span class="tex-span"><i>B</i></span> and <span class="tex-span"><i>C</i></span> from the range <span class="tex-span">[1, <i>N</i>]</span>, and it was asked to check whether the equation <span class="tex-span"><i>AB</i> = <i>C</i></span> is correct. Recently Billy studied the concept of a digital root of a number. We should remind you that a digital root <span class="tex-span"><i>d</i>(<i>x</i>)</span> of the number <span class="tex-span"><i>x</i></span> is the sum <span class="tex-span"><i>s</i>(<i>x</i>)</span> of all the digits of this number, if <span class="tex-span"><i>s</i>(<i>x</i>) ≤ 9</span>, otherwise it is <span class="tex-span"><i>d</i>(<i>s</i>(<i>x</i>))</span>. For example, a digital root of the number 6543 is calculated as follows: <span class="tex-span"><i>d</i>(6543) = <i>d</i>(6 + 5 + 4 + 3) = <i>d</i>(18) = 9</span>. Billy has counted that the digital root of a product of numbers is equal to the digital root of the product of the factors' digital roots, i.e. <span class="tex-span"><i>d</i>(<i>xy</i>) = <i>d</i>(<i>d</i>(<i>x</i>)<i>d</i>(<i>y</i>))</span>. And the following solution to the problem came to his mind: to calculate the digital roots and check if this condition is met. However, Billy has doubts that this condition is sufficient. That's why he asks you to find out the amount of test examples for the given problem such that the algorithm proposed by Billy makes mistakes.</p></div><div class="input-specification"><p>The first line contains the only number <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 10<sup class="upper-index">6</sup></span>).</p></div><div class="output-specification"><p>Output one number — the amount of required <span class="tex-span"><i>A</i></span>, <span class="tex-span"><i>B</i></span> and <span class="tex-span"><i>C</i></span> from the range <span class="tex-span">[1, <i>N</i>]</span>.</p></div>

## Input

<p>The first line contains the only number <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 10<sup class="upper-index">6</sup></span>).</p>

## Output

<p>Output one number — the amount of required <span class="tex-span"><i>A</i></span>, <span class="tex-span"><i>B</i></span> and <span class="tex-span"><i>C</i></span> from the range <span class="tex-span">[1, <i>N</i>]</span>.</p>





```input1
4

```




```input2
5

```




```output1
2

```




```output2
6

```



## Note

<p>For the first sample the required triples are <span class="tex-span">(3, 4, 3)</span> and <span class="tex-span">(4, 3, 3)</span>.</p>
