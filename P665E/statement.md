## Description

<div><p>One day, ZS the Coder wrote down an array of integers <span class="tex-span"><i>a</i></span> with elements <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>,  <i>a</i><sub class="lower-index">2</sub>,  ...,  <i>a</i><sub class="lower-index"><i>n</i></sub></span>.</p><p>A subarray of the array <span class="tex-span"><i>a</i></span> is a sequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>l</i></sub>,  <i>a</i><sub class="lower-index"><i>l</i>  +  1</sub>,  ...,  <i>a</i><sub class="lower-index"><i>r</i></sub></span> for some integers <span class="tex-span">(<i>l</i>,  <i>r</i>)</span> such that <span class="tex-span">1  ≤  <i>l</i>  ≤  <i>r</i>  ≤  <i>n</i></span>. ZS the Coder thinks that a subarray of <span class="tex-span"><i>a</i></span> is beautiful if the bitwise xor of all the elements in the subarray is at least <span class="tex-span"><i>k</i></span>.</p><p>Help ZS the Coder find the number of beautiful subarrays of <span class="tex-span"><i>a</i></span>!</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>, 1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of elements in the array <span class="tex-span"><i>a</i></span> and the value of the parameter <span class="tex-span"><i>k</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the elements of the array <span class="tex-span"><i>a</i></span>.</p></div><div class="output-specification"><p>Print the only integer <span class="tex-span"><i>c</i></span> — the number of beautiful subarrays of the array <span class="tex-span"><i>a</i></span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>, 1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of elements in the array <span class="tex-span"><i>a</i></span> and the value of the parameter <span class="tex-span"><i>k</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the elements of the array <span class="tex-span"><i>a</i></span>.</p>

## Output

<p>Print the only integer <span class="tex-span"><i>c</i></span> — the number of beautiful subarrays of the array <span class="tex-span"><i>a</i></span>.</p>





```input1
3 1
1 2 3

```




```input2
3 2
1 2 3

```




```input3
3 3
1 2 3

```




```output1
5

```




```output2
3

```




```output3
2

```


