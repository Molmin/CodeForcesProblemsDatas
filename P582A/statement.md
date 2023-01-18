## Description

<div><p>The GCD table <span class="tex-span"><i>G</i></span> of size <span class="tex-span"><i>n</i> × <i>n</i></span> for an array of positive integers <span class="tex-span"><i>a</i></span> of length <span class="tex-span"><i>n</i></span> is defined by formula </p><center> <img align="middle" class="tex-formula" src="file://oLoGHj3o.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Let us remind you that the greatest common divisor (GCD) of two positive integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> is the greatest integer that is divisor of both <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>, it is denoted as <img align="middle" class="tex-formula" src="file://10JOSEWg.png" style="max-width: 100.0%;max-height: 100.0%;">. For example, for array <span class="tex-span"><i>a</i> = {4, 3, 6, 2}</span> of length 4 the GCD table will look as follows:</p><center> <img class="tex-graphics" src="file://jstu0dYn.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Given all the numbers of the GCD table <span class="tex-span"><i>G</i></span>, restore array <span class="tex-span"><i>a</i></span>.</p></div><div class="input-specification"><p>The first line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500</span>) — the length of array <span class="tex-span"><i>a</i></span>. The second line contains <span class="tex-span"><i>n</i><sup class="upper-index">2</sup></span> space-separated numbers — the elements of the GCD table of <span class="tex-span"><i>G</i></span> for array <span class="tex-span"><i>a</i></span>. </p><p>All the numbers in the table are positive integers, not exceeding <span class="tex-span">10<sup class="upper-index">9</sup></span>. Note that the elements are given in an arbitrary order. It is guaranteed that the set of the input data corresponds to some array <span class="tex-span"><i>a</i></span>.</p></div><div class="output-specification"><p>In the single line print <span class="tex-span"><i>n</i></span> positive integers — the elements of array <span class="tex-span"><i>a</i></span>. If there are multiple possible solutions, you are allowed to print any of them.</p></div>

## Input

<p>The first line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500</span>) — the length of array <span class="tex-span"><i>a</i></span>. The second line contains <span class="tex-span"><i>n</i><sup class="upper-index">2</sup></span> space-separated numbers — the elements of the GCD table of <span class="tex-span"><i>G</i></span> for array <span class="tex-span"><i>a</i></span>. </p><p>All the numbers in the table are positive integers, not exceeding <span class="tex-span">10<sup class="upper-index">9</sup></span>. Note that the elements are given in an arbitrary order. It is guaranteed that the set of the input data corresponds to some array <span class="tex-span"><i>a</i></span>.</p>

## Output

<p>In the single line print <span class="tex-span"><i>n</i></span> positive integers — the elements of array <span class="tex-span"><i>a</i></span>. If there are multiple possible solutions, you are allowed to print any of them.</p>





```input1
4
2 1 2 3 4 3 2 6 1 1 2 2 1 2 3 2

```




```input2
1
42

```




```input3
2
1 1 1 1

```




```output1
4 3 6 2
```




```output2
42
```




```output3
1 1
```


