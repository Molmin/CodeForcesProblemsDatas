## Description

<div><p><span class="tex-font-style-underline">Petya loves lucky numbers. We all know that lucky numbers are the positive integers whose decimal representations contain only the lucky digits <span class="tex-font-style-bf">4</span> and <span class="tex-font-style-bf">7</span>. For example, numbers <span class="tex-font-style-bf">47</span>, <span class="tex-font-style-bf">744</span>, <span class="tex-font-style-bf">4</span> are lucky and <span class="tex-font-style-bf">5</span>, <span class="tex-font-style-bf">17</span>, <span class="tex-font-style-bf">467</span> are not.</span></p><p>Unfortunately, not all numbers are lucky. Petya calls a number <span class="tex-font-style-underline">nearly lucky</span> if the number of lucky digits in it is a lucky number. He wonders whether number <span class="tex-span"><i>n</i></span> is a nearly lucky number.</p></div><div class="input-specification"><p>The only line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup></span>).</p><p>Please do not use the %lld specificator to read or write 64-bit numbers in С++. It is preferred to use the cin, cout streams or the %I64d specificator.</p></div><div class="output-specification"><p>Print on the single line "<span class="tex-font-style-tt">YES</span>" if <span class="tex-span"><i>n</i></span> is a nearly lucky number. Otherwise, print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p></div>

## Input

<p>The only line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup></span>).</p><p>Please do not use the %lld specificator to read or write 64-bit numbers in С++. It is preferred to use the cin, cout streams or the %I64d specificator.</p>

## Output

<p>Print on the single line "<span class="tex-font-style-tt">YES</span>" if <span class="tex-span"><i>n</i></span> is a nearly lucky number. Otherwise, print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p>





```input1
40047

```




```input2
7747774

```




```input3
1000000000000000000

```




```output1
NO

```




```output2
YES

```




```output3
NO

```



## Note

<p>In the first sample there are 3 lucky digits (first one and last two), so the answer is "<span class="tex-font-style-tt">NO</span>".</p><p>In the second sample there are 7 lucky digits, 7 is lucky number, so the answer is "<span class="tex-font-style-tt">YES</span>".</p><p>In the third sample there are no lucky digits, so the answer is "<span class="tex-font-style-tt">NO</span>".</p>
