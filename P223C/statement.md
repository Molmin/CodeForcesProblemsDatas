## Description

<div><p>You've got an array <span class="tex-span"><i>a</i></span>, consisting of <span class="tex-span"><i>n</i></span> integers. The array elements are indexed from 1 to <span class="tex-span"><i>n</i></span>. Let's determine a two step operation like that:</p><ol> <li> First we build by the array <span class="tex-span"><i>a</i></span> an array <span class="tex-span"><i>s</i></span> of partial sums, consisting of <span class="tex-span"><i>n</i></span> elements. Element number <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) of array <span class="tex-span"><i>s</i></span> equals <img align="middle" class="tex-formula" src="file://edm5T4ed.png" style="max-width: 100.0%;max-height: 100.0%;">. The operation <span class="tex-span"><i>x</i>&nbsp;<i>mod</i>&nbsp;<i>y</i></span> means that we take the remainder of the division of number <span class="tex-span"><i>x</i></span> by number <span class="tex-span"><i>y</i></span>. </li><li> Then we write the contents of the array <span class="tex-span"><i>s</i></span> to the array <span class="tex-span"><i>a</i></span>. Element number <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) of the array <span class="tex-span"><i>s</i></span> becomes the <span class="tex-span"><i>i</i></span>-th element of the array <span class="tex-span"><i>a</i></span> (<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = <i>s</i><sub class="lower-index"><i>i</i></sub></span>). </li></ol><p>You task is to find array <span class="tex-span"><i>a</i></span> after exactly <span class="tex-span"><i>k</i></span> described operations are applied.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>). The next line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>&nbsp;— elements of the array <span class="tex-span"><i>a</i></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> integers &nbsp;— elements of the array <span class="tex-span"><i>a</i></span> after the operations are applied to it. Print the elements in the order of increasing of their indexes in the array <span class="tex-span"><i>a</i></span>. Separate the printed numbers by spaces.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>). The next line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>&nbsp;— elements of the array <span class="tex-span"><i>a</i></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> integers &nbsp;— elements of the array <span class="tex-span"><i>a</i></span> after the operations are applied to it. Print the elements in the order of increasing of their indexes in the array <span class="tex-span"><i>a</i></span>. Separate the printed numbers by spaces.</p>





```input1
3 1
1 2 3

```




```input2
5 0
3 14 15 92 6

```




```output1
1 3 6

```




```output2
3 14 15 92 6

```


