## Description

<div><p>Amr doesn't like Maths as he finds it really boring, so he usually sleeps in Maths lectures. But one day the teacher suspected that Amr is sleeping and asked him a question to make sure he wasn't.</p><p>First he gave Amr two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span>. Then he asked Amr, how many integer numbers <span class="tex-span"><i>x</i> &gt; 0</span> exist such that:</p><ul> <li> Decimal representation of <span class="tex-span"><i>x</i></span> (without leading zeroes) consists of exactly <span class="tex-span"><i>n</i></span> digits; </li><li> There exists some integer <span class="tex-span"><i>y</i> &gt; 0</span> such that: <ul> <li> <img align="middle" class="tex-formula" src="file://i8mrwWKI.png" style="max-width: 100.0%;max-height: 100.0%;">; </li><li> decimal representation of <span class="tex-span"><i>y</i></span> is a <span class="tex-font-style-it">suffix</span> of decimal representation of <span class="tex-span"><i>x</i></span>. </li></ul> </li></ul><p>As the answer to this question may be pretty huge the teacher asked Amr to output only its remainder modulo a number <span class="tex-span"><i>m</i></span>.</p><p>Can you help Amr escape this embarrassing situation?</p></div><div class="input-specification"><p>Input consists of three integers <span class="tex-span"><i>n</i>, <i>k</i>, <i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print the required number modulo <span class="tex-span"><i>m</i></span>.</p></div>

## Input

<p>Input consists of three integers <span class="tex-span"><i>n</i>, <i>k</i>, <i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print the required number modulo <span class="tex-span"><i>m</i></span>.</p>





```input1
1 2 1000

```




```input2
2 2 1000

```




```input3
5 3 1103

```




```output1
4
```




```output2
45
```




```output3
590
```



## Note

<p>A suffix of a string <span class="tex-span"><i>S</i></span> is a non-empty string that can be obtained by removing some number (possibly, zero) of first characters from <span class="tex-span"><i>S</i></span>.</p>
