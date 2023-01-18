## Description

<div><p>In this problem we'll use a stack which supports two types of operations:</p><ul> <li> Push a given number on the stack. </li><li> Pop two numbers from the stack, perform a given operation (addition or multiplication) on them and push the result on the stack. </li></ul><p>You are given a string which describes the sequence of operations to be performed on the stack. <span class="tex-span"><i>i</i></span>-th character corresponds to <span class="tex-span"><i>i</i></span>-th operation:</p><ul> <li> If <span class="tex-span"><i>i</i></span>-th character is a digit, push the corresponding number on the stack. </li><li> If <span class="tex-span"><i>i</i></span>-th character is «<span class="tex-font-style-tt">+</span>» or «<span class="tex-font-style-tt">*</span>», perform the corresponding operation. </li></ul><p>Initially the stack is empty. Output the topmost number on the stack after executing all given operations.</p></div><div class="input-specification"><p>The only line of input contains a string of operations, consisting of characters «<span class="tex-font-style-tt">+</span>», «<span class="tex-font-style-tt">*</span>» and digits (<span class="tex-font-style-tt">0..9</span>). The length of the string will be between 1 and 20 characters, inclusive.</p><p>The given sequence of operations is guaranteed to be correct, i.e. the stack will have at least two elements before every math operation. The numbers on the stack will never exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>. </p></div><div class="output-specification"><p>Output a single number — the topmost element of the stack after performing all given operations.</p></div>

## Input

<p>The only line of input contains a string of operations, consisting of characters «<span class="tex-font-style-tt">+</span>», «<span class="tex-font-style-tt">*</span>» and digits (<span class="tex-font-style-tt">0..9</span>). The length of the string will be between 1 and 20 characters, inclusive.</p><p>The given sequence of operations is guaranteed to be correct, i.e. the stack will have at least two elements before every math operation. The numbers on the stack will never exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>. </p>

## Output

<p>Output a single number — the topmost element of the stack after performing all given operations.</p>





```input1
12+3*66*+

```




```input2
149

```




```output1
45

```




```output2
9

```



## Note

<p>In the first case the stack will end up containing a single number — the result of calculating (1+2)*3+6*6.</p><p>In the second case there are no math operations, so the answer will be the last number pushed on the stack.</p>
