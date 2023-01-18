## Description

<div><p>Shakespeare is a widely known esoteric programming language in which programs look like plays by Shakespeare, and numbers are given by combinations of ornate epithets. In this problem we will have a closer look at the way the numbers are described in Shakespeare.</p><p>Each constant in Shakespeare is created from non-negative powers of 2 using arithmetic operations. For simplicity we'll allow only addition and subtraction and will look for a representation of the given number which requires a minimal number of operations.</p><p>You are given an integer <span class="tex-span"><i>n</i></span>. You have to represent it as <span class="tex-span"><i>n</i> = <i>a</i><sub class="lower-index">1</sub> + <i>a</i><sub class="lower-index">2</sub> + ... + <i>a</i><sub class="lower-index"><i>m</i></sub></span>, where each of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is a non-negative power of 2, possibly multiplied by -1. Find a representation which minimizes the value of <span class="tex-span"><i>m</i></span>.</p></div><div class="input-specification"><p>The only line of input contains a positive integer <span class="tex-span"><i>n</i></span>, written as its binary notation. The length of the notation is at most <span class="tex-span">10<sup class="upper-index">6</sup></span>. The first digit of the notation is guaranteed to be 1.</p></div><div class="output-specification"><p>Output the required minimal <span class="tex-span"><i>m</i></span>. After it output <span class="tex-span"><i>m</i></span> lines. Each line has to be formatted as "<span class="tex-font-style-tt">+2^x</span>" or "<span class="tex-font-style-tt">-2^x</span>", where <span class="tex-span"><i>x</i></span> is the power coefficient of the corresponding term. The order of the lines doesn't matter.</p></div>

## Input

<p>The only line of input contains a positive integer <span class="tex-span"><i>n</i></span>, written as its binary notation. The length of the notation is at most <span class="tex-span">10<sup class="upper-index">6</sup></span>. The first digit of the notation is guaranteed to be 1.</p>

## Output

<p>Output the required minimal <span class="tex-span"><i>m</i></span>. After it output <span class="tex-span"><i>m</i></span> lines. Each line has to be formatted as "<span class="tex-font-style-tt">+2^x</span>" or "<span class="tex-font-style-tt">-2^x</span>", where <span class="tex-span"><i>x</i></span> is the power coefficient of the corresponding term. The order of the lines doesn't matter.</p>





```input1
1111

```




```input2
1010011

```




```output1
2
+2^4
-2^0

```




```output2
4
+2^0
+2^1
+2^4
+2^6

```


