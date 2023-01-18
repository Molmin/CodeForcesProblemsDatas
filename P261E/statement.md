## Description

<div><p>Maxim has got a calculator. The calculator has two integer cells. Initially, the first cell contains number <span class="tex-span">1</span>, and the second cell contains number <span class="tex-span">0</span>. In one move you can perform one of the following operations:</p><ol> <li> Let's assume that at the current time the first cell contains number <span class="tex-span"><i>a</i></span>, and the second cell contains number <span class="tex-span"><i>b</i></span>. Write to the second cell number <span class="tex-span"><i>b</i> + 1</span>; </li><li> Let's assume that at the current time the first cell contains number <span class="tex-span"><i>a</i></span>, and the second cell contains number <span class="tex-span"><i>b</i></span>. Write to the first cell number <span class="tex-span"><i>a</i>·<i>b</i></span>. </li></ol><p>Maxim is wondering, how many integers <span class="tex-span"><i>x</i></span> <span class="tex-span">(<i>l</i> ≤ <i>x</i> ≤ <i>r</i>)</span> are there, such that we can write the number <span class="tex-span"><i>x</i></span> to the first cell of the calculator, having performed at most <span class="tex-span"><i>p</i></span> moves.</p></div><div class="input-specification"><p>The first line contains three integers: <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span>, <span class="tex-span"><i>p</i></span> <span class="tex-span">(2 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">9</sup>, 1 ≤ <i>p</i> ≤ 100)</span>. </p><p>The numbers in the line are separated by single spaces.</p></div><div class="output-specification"><p>In a single line print a single integer — the answer to the problem.</p></div>

## Input

<p>The first line contains three integers: <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span>, <span class="tex-span"><i>p</i></span> <span class="tex-span">(2 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">9</sup>, 1 ≤ <i>p</i> ≤ 100)</span>. </p><p>The numbers in the line are separated by single spaces.</p>

## Output

<p>In a single line print a single integer — the answer to the problem.</p>





```input1
2 10 3

```




```input2
2 111 100

```




```input3
2 111 11

```




```output1
1

```




```output2
106

```




```output3
47

```


