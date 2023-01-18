## Description

<div><p>Little Petya very much likes computers. Recently he has received a new "Ternatron IV" as a gift from his mother. Unlike other modern computers, "Ternatron IV" operates with ternary and not binary logic. Petya immediately wondered how the <span class="tex-span"><i>xor</i></span> operation is performed on this computer (and whether there is anything like it).</p><p>It turned out that the operation does exist (however, it is called <span class="tex-span"><i>tor</i></span>) and it works like this. Suppose that we need to calculate the value of the expression <span class="tex-span"><i>a</i> <i>tor</i> <i>b</i></span>. Both numbers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are written in the ternary notation one under the other one (<span class="tex-span"><i>b</i></span> under <span class="tex-span"><i>a</i></span>). If they have a different number of digits, then leading zeroes are added to the shorter number until the lengths are the same. Then the numbers are summed together digit by digit. The result of summing each two digits is calculated modulo 3. Note that there is no carry between digits (i. e. during this operation the digits aren't transferred). For example: <span class="tex-span">14<sub class="lower-index">10</sub> <i>tor</i> 50<sub class="lower-index">10</sub> = 0112<sub class="lower-index">3</sub> <i>tor</i> 1212<sub class="lower-index">3</sub> = 1021<sub class="lower-index">3</sub> = 34<sub class="lower-index">10</sub></span>.</p><p>Petya wrote numbers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>c</i></span> on a piece of paper. Help him find such number <span class="tex-span"><i>b</i></span>, that <span class="tex-span"><i>a</i> <i>tor</i> <i>b</i> = <i>c</i></span>. If there are several such numbers, print the smallest one.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">0 ≤ <i>a</i>, <i>c</i> ≤ 10<sup class="upper-index">9</sup></span>). Both numbers are written in decimal notation.</p></div><div class="output-specification"><p>Print the single integer <span class="tex-span"><i>b</i></span>, such that <span class="tex-span"><i>a</i> <i>tor</i> <i>b</i> = <i>c</i></span>. If there are several possible numbers <span class="tex-span"><i>b</i></span>, print the smallest one. You should print the number in decimal notation.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">0 ≤ <i>a</i>, <i>c</i> ≤ 10<sup class="upper-index">9</sup></span>). Both numbers are written in decimal notation.</p>

## Output

<p>Print the single integer <span class="tex-span"><i>b</i></span>, such that <span class="tex-span"><i>a</i> <i>tor</i> <i>b</i> = <i>c</i></span>. If there are several possible numbers <span class="tex-span"><i>b</i></span>, print the smallest one. You should print the number in decimal notation.</p>





```input1
14 34

```




```input2
50 34

```




```input3
387420489 225159023

```




```input4
5 5

```




```output1
50

```




```output2
14

```




```output3
1000000001

```




```output4
0

```


