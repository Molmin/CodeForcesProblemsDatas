## Description

<div><p>Roman is a young mathematician, very famous in Uzhland. Unfortunately, Sereja doesn't think so. To make Sereja change his mind, Roman is ready to solve any mathematical problem. After some thought, Sereja asked Roma to find, how many numbers are close to number <span class="tex-span"><i>n</i></span>, modulo <span class="tex-span"><i>m</i></span>.</p><p>Number <span class="tex-span"><i>x</i></span> is considered close to number <span class="tex-span"><i>n</i></span> modulo <span class="tex-span"><i>m</i></span>, if:</p><ul> <li> it can be obtained by rearranging the digits of number <span class="tex-span"><i>n</i></span>, </li><li> it doesn't have any leading zeroes, </li><li> the remainder after dividing number <span class="tex-span"><i>x</i></span> by <span class="tex-span"><i>m</i></span> equals 0. </li></ul><p>Roman is a good mathematician, but the number of such numbers is too huge for him. So he asks you to help him.</p><p> </p></div><div class="input-specification"><p>The first line contains two integers: <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> &lt; 10<sup class="upper-index">18</sup>)</span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 100)</span>.</p></div><div class="output-specification"><p>In a single line print a single integer — the number of numbers close to number <span class="tex-span"><i>n</i></span> modulo <span class="tex-span"><i>m</i></span>.</p></div>

## Input

<p>The first line contains two integers: <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> &lt; 10<sup class="upper-index">18</sup>)</span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 100)</span>.</p>

## Output

<p>In a single line print a single integer — the number of numbers close to number <span class="tex-span"><i>n</i></span> modulo <span class="tex-span"><i>m</i></span>.</p>





```input1
104 2

```




```input2
223 4

```




```input3
7067678 8

```




```output1
3

```




```output2
1

```




```output3
47

```



## Note

<p>In the first sample the required numbers are: 104, 140, 410.</p><p>In the second sample the required number is 232.</p>
