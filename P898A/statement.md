## Description

<div><p>Vasya has a non-negative integer <span class="tex-span"><i>n</i></span>. He wants to round it to nearest integer, which ends up with <span class="tex-span">0</span>. If <span class="tex-span"><i>n</i></span> already ends up with <span class="tex-span">0</span>, Vasya considers it already rounded.</p><p>For example, if <span class="tex-span"><i>n</i> = 4722</span> answer is <span class="tex-span">4720</span>. If <span class="tex-span"><i>n</i> = 5</span> Vasya can round it to <span class="tex-span">0</span> or to <span class="tex-span">10</span>. Both ways are correct.</p><p>For given <span class="tex-span"><i>n</i></span> find out to which integer will Vasya round it.</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— number that Vasya has.</p></div><div class="output-specification"><p>Print result of rounding <span class="tex-span"><i>n</i></span>. Pay attention that in some cases answer isn't unique. In that case print any correct answer.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— number that Vasya has.</p>

## Output

<p>Print result of rounding <span class="tex-span"><i>n</i></span>. Pay attention that in some cases answer isn't unique. In that case print any correct answer.</p>





```input1
5

```




```input2
113

```




```input3
1000000000

```




```input4
5432359

```




```output1
0

```




```output2
110

```




```output3
1000000000

```




```output4
5432360

```



## Note

<p>In the first example <span class="tex-span"><i>n</i> = 5</span>. Nearest integers, that ends up with zero are <span class="tex-span">0</span> and <span class="tex-span">10</span>. Any of these answers is correct, so you can print <span class="tex-span">0</span> or <span class="tex-span">10</span>.</p>
