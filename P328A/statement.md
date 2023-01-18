## Description

<div><p>Petya is preparing for IQ test and he has noticed that there many problems like: <span class="tex-font-style-it">you are given a sequence, find the next number.</span> Now Petya can solve only problems with arithmetic or geometric progressions.</p><p><span class="tex-font-style-it">Arithmetic progression</span> is a sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> + <i>d</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> + 2<i>d</i></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> + (<i>n</i> - 1)<i>d</i></span>, where <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>d</i></span> are any numbers.</p><p><span class="tex-font-style-it">Geometric progression</span> is a sequence <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index">2</sub> = <i>b</i><sub class="lower-index">1</sub><i>q</i></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>n</i></sub> = <i>b</i><sub class="lower-index"><i>n</i> - 1</sub><i>q</i></span>, where <span class="tex-span"><i>b</i><sub class="lower-index">1</sub> ≠ 0</span>, <span class="tex-span"><i>q</i> ≠ 0</span>, <span class="tex-span"><i>q</i> ≠ 1</span>. </p><p>Help Petya and write a program to determine if the given sequence is arithmetic or geometric. Also it should found the next number. If the sequence is neither arithmetic nor geometric, print 42 (he thinks it is impossible to find better answer). You should also print 42 if the next element of progression is not integer. So answer is always integer.</p></div><div class="input-specification"><p>The first line contains exactly four integer numbers between 1 and 1000, inclusively.</p></div><div class="output-specification"><p>Print the required number. If the given sequence is arithmetic progression, print the next progression element. Similarly, if the given sequence is geometric progression, print the next progression element.</p><p>Print 42 if the given sequence is not an arithmetic or geometric progression.</p></div>

## Input

<p>The first line contains exactly four integer numbers between 1 and 1000, inclusively.</p>

## Output

<p>Print the required number. If the given sequence is arithmetic progression, print the next progression element. Similarly, if the given sequence is geometric progression, print the next progression element.</p><p>Print 42 if the given sequence is not an arithmetic or geometric progression.</p>





```input1
836 624 412 200

```




```input2
1 334 667 1000

```




```output1
-12

```




```output2
1333

```



## Note

<p>This problem contains very weak pretests!</p>
