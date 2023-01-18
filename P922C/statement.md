## Description

<div><p>Imp is watching a documentary about cave painting.</p><center> <img class="tex-graphics" src="file://33kp7VE5.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Some numbers, carved in chaotic order, immediately attracted his attention. Imp rapidly proposed a guess that they are the remainders of division of a number <span class="tex-span"><i>n</i></span> by all integers <span class="tex-span"><i>i</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i></span>. Unfortunately, there are too many integers to analyze for Imp.</p><p>Imp wants you to check whether all these remainders are distinct. Formally, he wants to check, if all <img align="middle" class="tex-formula" src="file://GsyJpu48.png" style="max-width: 100.0%;max-height: 100.0%;">, <span class="tex-span">1 ≤ <i>i</i> ≤ <i>k</i></span>, are distinct, i.&nbsp;e. there is no such pair <span class="tex-span">(<i>i</i>, <i>j</i>)</span> that: </p><ul> <li> <span class="tex-span">1 ≤ <i>i</i> &lt; <i>j</i> ≤ <i>k</i></span>, </li><li> <img align="middle" class="tex-formula" src="file://rxWDemex.png" style="max-width: 100.0%;max-height: 100.0%;">, where <img align="middle" class="tex-formula" src="file://jStULqfB.png" style="max-width: 100.0%;max-height: 100.0%;"> is the remainder of division <span class="tex-span"><i>x</i></span> by <span class="tex-span"><i>y</i></span>. </li></ul></div><div class="input-specification"><p>The only line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>k</i> ≤ 10<sup class="upper-index">18</sup>)</span>.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">Yes</span>", if all the remainders are distinct, and "<span class="tex-font-style-tt">No</span>" otherwise.</p><p>You can print each letter in arbitrary case (lower or upper).</p></div>

## Input

<p>The only line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>k</i> ≤ 10<sup class="upper-index">18</sup>)</span>.</p>

## Output

<p>Print "<span class="tex-font-style-tt">Yes</span>", if all the remainders are distinct, and "<span class="tex-font-style-tt">No</span>" otherwise.</p><p>You can print each letter in arbitrary case (lower or upper).</p>





```input1
4 4

```




```input2
5 3

```




```output1
No

```




```output2
Yes

```



## Note

<p>In the first sample remainders modulo <span class="tex-span">1</span> and <span class="tex-span">4</span> coincide.</p>
