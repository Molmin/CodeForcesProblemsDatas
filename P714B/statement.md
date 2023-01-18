## Description

<div><p>Today, hedgehog Filya went to school for the very first time! Teacher gave him a homework which Filya was unable to complete without your help.</p><p>Filya is given an array of non-negative integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. First, he pick an integer <span class="tex-span"><i>x</i></span> and then he adds <span class="tex-span"><i>x</i></span> to some elements of the array (no more than once), subtract <span class="tex-span"><i>x</i></span> from some other elements (also, no more than once) and do no change other elements. He wants all elements of the array to be equal.</p><p>Now he wonders if it's possible to pick such integer <span class="tex-span"><i>x</i></span> and change some elements of the array using this <span class="tex-span"><i>x</i></span> in order to make all elements equal.</p></div><div class="input-specification"><p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of integers in the Filya's array. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— elements of the array.</p></div><div class="output-specification"><p>If it's impossible to make all elements of the array equal using the process given in the problem statement, then print "<span class="tex-font-style-tt">NO</span>" (without quotes) in the only line of the output. Otherwise print "<span class="tex-font-style-tt">YES</span>" (without quotes).</p></div>

## Input

<p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of integers in the Filya's array. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— elements of the array.</p>

## Output

<p>If it's impossible to make all elements of the array equal using the process given in the problem statement, then print "<span class="tex-font-style-tt">NO</span>" (without quotes) in the only line of the output. Otherwise print "<span class="tex-font-style-tt">YES</span>" (without quotes).</p>





```input1
5
1 3 3 2 1

```




```input2
5
1 2 3 4 5

```




```output1
YES

```




```output2
NO

```



## Note

<p>In the first sample Filya should select <span class="tex-span"><i>x</i> = 1</span>, then add it to the first and the last elements of the array and subtract from the second and the third elements.</p>
