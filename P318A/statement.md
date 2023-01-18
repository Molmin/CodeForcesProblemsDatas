## Description

<div><p>Being a nonconformist, Volodya is displeased with the current state of things, particularly with the order of natural numbers (natural number is positive integer number). He is determined to rearrange them. But there are too many natural numbers, so Volodya decided to start with the first <span class="tex-span"><i>n</i></span>. He writes down the following sequence of numbers: firstly all odd integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> (in ascending order), then all even integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> (also in ascending order). Help our hero to find out which number will stand at the position number <span class="tex-span"><i>k</i></span>.</p></div><div class="input-specification"><p>The only line of input contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">12</sup></span>).</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in C++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div><div class="output-specification"><p>Print the number that will stand at the position number <span class="tex-span"><i>k</i></span> after Volodya's manipulations.</p></div>

## Input

<p>The only line of input contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">12</sup></span>).</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in C++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>

## Output

<p>Print the number that will stand at the position number <span class="tex-span"><i>k</i></span> after Volodya's manipulations.</p>





```input1
10 3

```




```input2
7 7

```




```output1
5
```




```output2
6
```



## Note

<p>In the first sample Volodya's sequence will look like this: {1, 3, 5, 7, 9, 2, 4, 6, 8, 10}. The third place in the sequence is therefore occupied by the number 5.</p>
