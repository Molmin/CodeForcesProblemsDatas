## Description

<div><p>Dreamoon saw a large integer <span class="tex-span"><i>x</i></span> written on the ground and wants to print its binary form out. Dreamoon has accomplished the part of turning <span class="tex-span"><i>x</i></span> into its binary format. Now he is going to print it in the following manner.</p><p>He has an integer <span class="tex-span"><i>n</i> = 0</span> and can only perform the following two operations in any order for unlimited times each:</p><ol> <li> Print n in binary form without leading zeros, each print will append to the right of previous prints. </li><li> Increase n by 1. </li></ol><p>Let's define an <span class="tex-font-style-it">ideal sequence</span> as a sequence of operations that can successfully print binary representation of <span class="tex-span"><i>x</i></span> without leading zeros and ends with a print operation (i.e. operation 1). Dreamoon wants to know how many different ideal sequences are there and the length (in operations) of the shortest ideal sequence.</p><p>The answers might be large so please print them modulo 1000000007 (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p><p>Let's define the string representation of an ideal sequence as a string of <span class="tex-font-style-tt">'1'</span> and <span class="tex-font-style-tt">'2'</span> where the <span class="tex-span"><i>i</i></span>-th character in the string matches the <span class="tex-span"><i>i</i></span>-th operation performed. Two ideal sequences are called different if their string representations are different.</p></div><div class="input-specification"><p>The single line of the input contains a binary integer representing <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> &lt; 2<sup class="upper-index">5000</sup></span>) without leading zeros.</p></div><div class="output-specification"><p>The first line of the output should contain an integer representing the number of different ideal sequences modulo 1000000007 (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p><p>The second line of the output contains an integer representing the minimal length of an ideal sequence modulo 1000000007 (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div>

## Input

<p>The single line of the input contains a binary integer representing <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> &lt; 2<sup class="upper-index">5000</sup></span>) without leading zeros.</p>

## Output

<p>The first line of the output should contain an integer representing the number of different ideal sequences modulo 1000000007 (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p><p>The second line of the output contains an integer representing the minimal length of an ideal sequence modulo 1000000007 (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p>





```input1
101

```




```input2
11010

```




```output1
1
6

```




```output2
3
5

```



## Note

<p>For the first sample, the shortest and the only ideal sequence is «<span class="tex-font-style-tt">222221</span>» of length <span class="tex-span">6</span>.</p><p>For the second sample, there are three ideal sequences «<span class="tex-font-style-tt">21211</span>», «<span class="tex-font-style-tt">212222222221</span>», «<span class="tex-font-style-tt">222222222222222222222222221</span>». Among them the shortest one has length <span class="tex-span">5</span>.</p>
