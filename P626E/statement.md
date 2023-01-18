## Description

<div><p>Define the <span class="tex-font-style-it">simple skewness</span> of a collection of numbers to be the collection's mean minus its median. You are given a list of <span class="tex-span"><i>n</i></span> (not necessarily distinct) integers. Find the non-empty subset (with repetition) with the maximum simple skewness.</p><p>The mean of a collection is the average of its elements. The median of a collection is its middle element when all of its elements are sorted, or the average of its two middle elements if it has even size.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of elements in the list.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>)&nbsp;— the <span class="tex-span"><i>i</i></span>th element of the list.</p></div><div class="output-specification"><p>In the first line, print a single integer <span class="tex-span"><i>k</i></span>&nbsp;— the size of the subset.</p><p>In the second line, print <span class="tex-span"><i>k</i></span> integers&nbsp;— the elements of the subset in any order.</p><p>If there are multiple optimal subsets, print any.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of elements in the list.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>)&nbsp;— the <span class="tex-span"><i>i</i></span>th element of the list.</p>

## Output

<p>In the first line, print a single integer <span class="tex-span"><i>k</i></span>&nbsp;— the size of the subset.</p><p>In the second line, print <span class="tex-span"><i>k</i></span> integers&nbsp;— the elements of the subset in any order.</p><p>If there are multiple optimal subsets, print any.</p>





```input1
4
1 2 3 12

```




```input2
4
1 1 2 2

```




```input3
2
1 2

```




```output1
3
1 2 12 

```




```output2
3
1 1 2 

```




```output3
2
1 2

```



## Note

<p>In the first case, the optimal subset is <img align="middle" class="tex-formula" src="file://VatE5jBW.png" style="max-width: 100.0%;max-height: 100.0%;">, which has mean <span class="tex-span">5</span>, median <span class="tex-span">2</span>, and simple skewness of <span class="tex-span">5 - 2 = 3</span>.</p><p>In the second case, the optimal subset is <img align="middle" class="tex-formula" src="file://RKuJnonU.png" style="max-width: 100.0%;max-height: 100.0%;">. Note that repetition is allowed.</p><p>In the last case, any subset has the same median and mean, so all have simple skewness of <span class="tex-span">0</span>.</p>
