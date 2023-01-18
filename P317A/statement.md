## Description

<div><p>Let us call a pair of integer numbers <span class="tex-font-style-it"><span class="tex-span"><i>m</i></span>-perfect</span>, if at least one number in the pair is greater than or equal to <span class="tex-span"><i>m</i></span>. Thus, the pairs (3, 3) and (0, 2) are 2-perfect while the pair (-1, 1) is not.</p><p>Two integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> are written on the blackboard. It is allowed to erase one of them and replace it with the sum of the numbers, <span class="tex-span">(<i>x</i> + <i>y</i>)</span>.</p><p>What is the minimum number of such operations one has to perform in order to make the given pair of integers <span class="tex-span"><i>m</i></span>-perfect?</p></div><div class="input-specification"><p>Single line of the input contains three integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span"> - 10<sup class="upper-index">18</sup> ≤ <i>x</i></span>, <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>m</i> ≤ 10<sup class="upper-index">18</sup></span>).</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in C++. It is preffered to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div><div class="output-specification"><p>Print the minimum number of operations or "<span class="tex-font-style-tt">-1</span>" (without quotes), if it is impossible to transform the given pair to the <span class="tex-span"><i>m</i></span>-perfect one.</p></div>

## Input

<p>Single line of the input contains three integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span"> - 10<sup class="upper-index">18</sup> ≤ <i>x</i></span>, <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>m</i> ≤ 10<sup class="upper-index">18</sup></span>).</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in C++. It is preffered to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>

## Output

<p>Print the minimum number of operations or "<span class="tex-font-style-tt">-1</span>" (without quotes), if it is impossible to transform the given pair to the <span class="tex-span"><i>m</i></span>-perfect one.</p>





```input1
1 2 5

```




```input2
-1 4 15

```




```input3
0 -1 5

```




```output1
2

```




```output2
4

```




```output3
-1

```



## Note

<p>In the first sample the following sequence of operations is suitable: (1, 2) <img align="middle" class="tex-formula" src="file://hxQxwh4S.png" style="max-width: 100.0%;max-height: 100.0%;"> (3, 2) <img align="middle" class="tex-formula" src="file://6EyON4Q8.png" style="max-width: 100.0%;max-height: 100.0%;"> (5, 2).</p><p>In the second sample: (-1, 4) <img align="middle" class="tex-formula" src="file://7WYQAHDE.png" style="max-width: 100.0%;max-height: 100.0%;"> (3, 4) <img align="middle" class="tex-formula" src="file://K0BZvLGe.png" style="max-width: 100.0%;max-height: 100.0%;"> (7, 4) <img align="middle" class="tex-formula" src="file://lleXqQXR.png" style="max-width: 100.0%;max-height: 100.0%;"> (11, 4) <img align="middle" class="tex-formula" src="file://63CsU1Jk.png" style="max-width: 100.0%;max-height: 100.0%;"> (15, 4).</p><p>Finally, in the third sample <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> cannot be made positive, hence there is no proper sequence of operations.</p>
