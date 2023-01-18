## Description

<div><p>Misha has an array of integers of length <span class="tex-span"><i>n</i></span>. He wants to choose <span class="tex-span"><i>k</i></span> different continuous subarrays, so that each element of the array belongs to at least one of the chosen subarrays.</p><p>Misha wants to choose the subarrays in such a way that if he calculated the sum of elements for each subarray, and then add up all these sums, the resulting value was maximum possible.</p></div><div class="input-specification"><p>The first line of input contains two integers: <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i>·(<i>n</i> + 1) / 2</span>)&nbsp;— the number of elements in the array and the number of different subarrays that must be chosen.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 50 000 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 50 000</span>)&nbsp;— the elements of the array.</p></div><div class="output-specification"><p>Output one integer&nbsp;— the maximum possible value Misha can get by choosing <span class="tex-span"><i>k</i></span> different subarrays.</p></div>

## Input

<p>The first line of input contains two integers: <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i>·(<i>n</i> + 1) / 2</span>)&nbsp;— the number of elements in the array and the number of different subarrays that must be chosen.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 50 000 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 50 000</span>)&nbsp;— the elements of the array.</p>

## Output

<p>Output one integer&nbsp;— the maximum possible value Misha can get by choosing <span class="tex-span"><i>k</i></span> different subarrays.</p>





```input1
5 4
6 -4 -10 -4 7

```




```output1
11

```


