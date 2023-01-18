## Description

<div><p>For each positive integer <span class="tex-span"><i>n</i></span> consider the integer <span class="tex-span">ψ(<i>n</i>)</span> which is obtained from <span class="tex-span"><i>n</i></span> by replacing every digit <span class="tex-span"><i>a</i></span> in the decimal notation of <span class="tex-span"><i>n</i></span> with the digit <span class="tex-span">(9  -  <i>a</i>)</span>. We say that <span class="tex-span">ψ(<i>n</i>)</span> is the <span class="tex-font-style-it">reflection</span> of <span class="tex-span"><i>n</i></span>. For example, reflection of <span class="tex-span">192</span> equals <span class="tex-span">807</span>. Note that leading zeros (if any) should be omitted. So reflection of <span class="tex-span">9</span> equals <span class="tex-span">0</span>, reflection of <span class="tex-span">91</span> equals <span class="tex-span">8</span>.</p><p>Let us call the <span class="tex-font-style-it">weight</span> of the number the product of the number and its reflection. Thus, the weight of the number <span class="tex-span">10</span> is equal to <span class="tex-span">10·89 = 890</span>.</p><p>Your task is to find the maximum weight of the numbers in the given range <span class="tex-span">[<i>l</i>, <i>r</i>]</span> (boundaries are included).</p></div><div class="input-specification"><p>Input contains two space-separated integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">9</sup></span>) — bounds of the range.</p></div><div class="output-specification"><p>Output should contain single integer number: maximum value of the product <span class="tex-span"><i>n</i>·ψ(<i>n</i>)</span>, where <span class="tex-span"><i>l</i> ≤ <i>n</i> ≤ <i>r</i></span>.</p><p>Please, do not use <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preferred to use <span class="tex-font-style-tt">cout</span> (also you may use <span class="tex-font-style-tt">%I64d</span>).</p></div>

## Input

<p>Input contains two space-separated integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">9</sup></span>) — bounds of the range.</p>

## Output

<p>Output should contain single integer number: maximum value of the product <span class="tex-span"><i>n</i>·ψ(<i>n</i>)</span>, where <span class="tex-span"><i>l</i> ≤ <i>n</i> ≤ <i>r</i></span>.</p><p>Please, do not use <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preferred to use <span class="tex-font-style-tt">cout</span> (also you may use <span class="tex-font-style-tt">%I64d</span>).</p>





```input1
3 7

```




```input2
1 1

```




```input3
8 10

```




```output1
20
```




```output2
8
```




```output3
890
```



## Note

<p>In the third sample weight of <span class="tex-span">8</span> equals <span class="tex-span">8·1 = 8</span>, weight of <span class="tex-span">9</span> equals <span class="tex-span">9·0 = 0</span>, weight of <span class="tex-span">10</span> equals <span class="tex-span">890</span>.</p><p>Thus, maximum value of the product is equal to <span class="tex-span">890</span>.</p>
