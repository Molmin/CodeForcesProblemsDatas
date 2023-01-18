## Description

<div><p>We all know that GukiZ often plays with arrays. </p><p>Now he is thinking about this problem: how many arrays <span class="tex-span"><i>a</i></span>, of length <span class="tex-span"><i>n</i></span>, with non-negative elements <span class="tex-font-style-bf">strictly less</span> then <span class="tex-span">2<sup class="upper-index"><i>l</i></sup></span> meet the following condition: <img align="middle" class="tex-formula" src="file://FGcCcwcc.png" style="max-width: 100.0%;max-height: 100.0%;">? Here operation <img align="middle" class="tex-formula" src="file://WAhJ1BQX.png" style="max-width: 100.0%;max-height: 100.0%;"> means bitwise AND (in <span class="tex-font-style-tt">Pascal</span> it is equivalent to <span class="tex-font-style-tt">and</span>, in <span class="tex-font-style-tt">C/C++/Java/Python</span> it is equivalent to <span class="tex-font-style-tt">&amp;</span>), operation <img align="middle" class="tex-formula" src="file://cK3Z7ZIM.png" style="max-width: 100.0%;max-height: 100.0%;"> means bitwise OR (in <span class="tex-font-style-tt">Pascal</span> it is equivalent to <img align="middle" class="tex-formula" src="file://1oSMVos9.png" style="max-width: 100.0%;max-height: 100.0%;">, in <span class="tex-font-style-tt">C/C++/Java/Python</span> it is equivalent to <span class="tex-font-style-tt">|</span>). </p><p>Because the answer can be quite large, calculate it modulo <span class="tex-span"><i>m</i></span>. This time GukiZ hasn't come up with solution, and needs you to help him!</p></div><div class="input-specification"><p>First and the only line of input contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span">0 ≤ <i>l</i> ≤ 64</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup> + 7</span>).</p></div><div class="output-specification"><p>In the single line print the number of arrays satisfying the condition above modulo <span class="tex-span"><i>m</i></span>.</p></div>

## Input

<p>First and the only line of input contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span">0 ≤ <i>l</i> ≤ 64</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup> + 7</span>).</p>

## Output

<p>In the single line print the number of arrays satisfying the condition above modulo <span class="tex-span"><i>m</i></span>.</p>





```input1
2 1 2 10

```




```input2
2 1 1 3

```




```input3
3 3 2 10

```




```output1
3

```




```output2
1

```




```output3
9

```



## Note

<p>In the first sample, satisfying arrays are <span class="tex-span">{1, 1}, {3, 1}, {1, 3}</span>.</p><p>In the second sample, only satisfying array is <span class="tex-span">{1, 1}</span>.</p><p>In the third sample, satisfying arrays are <span class="tex-span">{0, 3, 3}, {1, 3, 2}, {1, 3, 3}, {2, 3, 1}, {2, 3, 3}, {3, 3, 0}, {3, 3, 1}, {3, 3, 2}, {3, 3, 3}</span>.</p>
