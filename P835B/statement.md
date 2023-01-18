## Description

<div><p>Some natural number was written on the board. Its sum of digits was not less than <span class="tex-span"><i>k</i></span>. But you were distracted a bit, and someone changed this number to <span class="tex-span"><i>n</i></span>, replacing some digits with others. It's known that the length of the number didn't change.</p><p>You have to find the minimum number of digits in which these two numbers can differ.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The second line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> &lt; 10<sup class="upper-index">100000</sup></span>).</p><p>There are no leading zeros in <span class="tex-span"><i>n</i></span>. It's guaranteed that this situation is possible.</p></div><div class="output-specification"><p>Print the minimum number of digits in which the initial number and <span class="tex-span"><i>n</i></span> can differ.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The second line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> &lt; 10<sup class="upper-index">100000</sup></span>).</p><p>There are no leading zeros in <span class="tex-span"><i>n</i></span>. It's guaranteed that this situation is possible.</p>

## Output

<p>Print the minimum number of digits in which the initial number and <span class="tex-span"><i>n</i></span> can differ.</p>





```input1
3
11

```




```input2
3
99

```




```output1
1

```




```output2
0

```



## Note

<p>In the first example, the initial number could be <span class="tex-span">12</span>.</p><p>In the second example the sum of the digits of <span class="tex-span"><i>n</i></span> is not less than <span class="tex-span"><i>k</i></span>. The initial number could be equal to <span class="tex-span"><i>n</i></span>.</p>
