## Description

<div><p>Consider the infinite sequence of integers: <span class="tex-span">1, 1, 2, 1, 2, 3, 1, 2, 3, 4, 1, 2, 3, 4, 5...</span>. The sequence is built in the following way: at first the number <span class="tex-span">1</span> is written out, then the numbers from <span class="tex-span">1</span> to <span class="tex-span">2</span>, then the numbers from <span class="tex-span">1</span> to <span class="tex-span">3</span>, then the numbers from <span class="tex-span">1</span> to <span class="tex-span">4</span> and so on. Note that the sequence contains numbers, not digits. For example number <span class="tex-span">10</span> first appears in the sequence in position <span class="tex-span">55</span> (the elements are numerated from one).</p><p>Find the number on the <span class="tex-span"><i>n</i></span>-th position of the sequence.</p></div><div class="input-specification"><p>The only line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">14</sup></span>) — the position of the number to find.</p><p>Note that the given number is too large, so you should use <span class="tex-span">64</span>-bit integer type to store it. In <span class="tex-font-style-tt">C++</span> you can use the <span class="tex-font-style-tt">long long</span> integer type and in <span class="tex-font-style-tt">Java</span> you can use <span class="tex-font-style-tt">long</span> integer type.</p></div><div class="output-specification"><p>Print the element in the <span class="tex-span"><i>n</i></span>-th position of the sequence (the elements are numerated from one).</p></div>

## Input

<p>The only line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">14</sup></span>) — the position of the number to find.</p><p>Note that the given number is too large, so you should use <span class="tex-span">64</span>-bit integer type to store it. In <span class="tex-font-style-tt">C++</span> you can use the <span class="tex-font-style-tt">long long</span> integer type and in <span class="tex-font-style-tt">Java</span> you can use <span class="tex-font-style-tt">long</span> integer type.</p>

## Output

<p>Print the element in the <span class="tex-span"><i>n</i></span>-th position of the sequence (the elements are numerated from one).</p>





```input1
3

```




```input2
5

```




```input3
10

```




```input4
55

```




```input5
56

```




```output1
2

```




```output2
2

```




```output3
4

```




```output4
10

```




```output5
1

```


