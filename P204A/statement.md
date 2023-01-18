## Description

<div><p>The Little Elephant very much loves sums on intervals.</p><p>This time he has a pair of integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> <span class="tex-span">(<i>l</i> ≤ <i>r</i>)</span>. The Little Elephant has to find the number of such integers <span class="tex-span"><i>x</i></span> <span class="tex-span">(<i>l</i> ≤ <i>x</i> ≤ <i>r</i>)</span>, that the first digit of integer <span class="tex-span"><i>x</i></span> equals the last one (in decimal notation). For example, such numbers as <span class="tex-span">101</span>, <span class="tex-span">477474</span> or <span class="tex-span">9</span> will be included in the answer and <span class="tex-span">47</span>, <span class="tex-span">253</span> or <span class="tex-span">1020</span> will not.</p><p>Help him and count the number of described numbers <span class="tex-span"><i>x</i></span> for a given pair <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span>.</p></div><div class="input-specification"><p>The single line contains a pair of integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> <span class="tex-span">(1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">18</sup>)</span> — the boundaries of the interval.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div><div class="output-specification"><p>On a single line print a single integer — the answer to the problem.</p></div>

## Input

<p>The single line contains a pair of integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> <span class="tex-span">(1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">18</sup>)</span> — the boundaries of the interval.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>

## Output

<p>On a single line print a single integer — the answer to the problem.</p>





```input1
2 47

```




```input2
47 1024

```




```output1
12

```




```output2
98

```



## Note

<p>In the first sample the answer includes integers <span class="tex-font-style-tt">2, 3, 4, 5, 6, 7, 8, 9, 11, 22, 33, 44</span>. </p>
