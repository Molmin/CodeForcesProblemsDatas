## Description

<div><p>Recently Maxim has found an array of <span class="tex-span"><i>n</i></span> integers, needed by no one. He immediately come up with idea of changing it: he invented positive integer <span class="tex-span"><i>x</i></span> and decided to add or subtract it from arbitrary array elements. Formally, by applying single operation Maxim chooses integer <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) and replaces the <span class="tex-span"><i>i</i></span>-th element of array <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> either with <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> + <i>x</i></span> or with <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> - <i>x</i></span>. Please note that the operation may be applied more than once to the same position.</p><p>Maxim is a curious minimalis, thus he wants to know what is the minimum value that the product of all array elements (i.e. <img align="middle" class="tex-formula" src="file://29j5bRNA.png" style="max-width: 100.0%;max-height: 100.0%;">) can reach, if Maxim would apply no more than <span class="tex-span"><i>k</i></span> operations to it. Please help him in that.</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>n</i>, <i>k</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 200 000, 1 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of elements in the array, the maximum number of operations and the number invented by Maxim, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<img align="middle" class="tex-formula" src="file://N37GDNA6.png" style="max-width: 100.0%;max-height: 100.0%;">)&nbsp;— the elements of the array found by Maxim.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> in the only line&nbsp;— the array elements after applying no more than <span class="tex-span"><i>k</i></span> operations to the array. In particular, <img align="middle" class="tex-formula" src="file://pxg5fDXi.png" style="max-width: 100.0%;max-height: 100.0%;"> should stay true for every <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>, but the product of all array elements should be <span class="tex-font-style-bf">minimum possible</span>.</p><p>If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>n</i>, <i>k</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 200 000, 1 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of elements in the array, the maximum number of operations and the number invented by Maxim, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<img align="middle" class="tex-formula" src="file://N37GDNA6.png" style="max-width: 100.0%;max-height: 100.0%;">)&nbsp;— the elements of the array found by Maxim.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> in the only line&nbsp;— the array elements after applying no more than <span class="tex-span"><i>k</i></span> operations to the array. In particular, <img align="middle" class="tex-formula" src="file://pxg5fDXi.png" style="max-width: 100.0%;max-height: 100.0%;"> should stay true for every <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>, but the product of all array elements should be <span class="tex-font-style-bf">minimum possible</span>.</p><p>If there are multiple answers, print any of them.</p>





```input1
5 3 1
5 4 3 5 2

```




```input2
5 3 1
5 4 3 5 5

```




```input3
5 3 1
5 4 4 5 5

```




```input4
3 2 7
5 4 2

```




```output1
5 4 3 5 -1 

```




```output2
5 4 0 5 5 

```




```output3
5 1 4 5 5 

```




```output4
5 11 -5 

```


