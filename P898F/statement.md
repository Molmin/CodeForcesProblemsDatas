## Description

<div><p>A correct expression of the form <span class="tex-font-style-tt">a+b=c</span> was written; <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> are non-negative integers without leading zeros. In this expression, the plus and equally signs were lost. The task is to restore the expression. In other words, one character '<span class="tex-font-style-tt">+</span>' and one character '<span class="tex-font-style-tt">=</span>' should be inserted into given sequence of digits so that: </p><ul> <li> character'<span class="tex-font-style-tt">+</span>' is placed on the left of character '<span class="tex-font-style-tt">=</span>', </li><li> characters '<span class="tex-font-style-tt">+</span>' and '<span class="tex-font-style-tt">=</span>' split the sequence into three non-empty subsequences consisting of digits (let's call the left part <span class="tex-font-style-tt">a</span>, the middle part&nbsp;— <span class="tex-font-style-tt">b</span> and the right part&nbsp;— <span class="tex-font-style-tt">c</span>), </li><li> all the three parts <span class="tex-font-style-tt">a</span>, <span class="tex-font-style-tt">b</span> and <span class="tex-font-style-tt">c</span> do not contain leading zeros, </li><li> it is true that <span class="tex-font-style-tt">a+b=c</span>. </li></ul><p>It is guaranteed that in given tests answer always exists.</p></div><div class="input-specification"><p>The first line contains a non-empty string consisting of digits. The length of the string does not exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p></div><div class="output-specification"><p>Output the restored expression. If there are several solutions, you can print any of them.</p><p>Note that the answer <span class="tex-font-style-bf">at first</span> should contain two terms (divided with symbol '<span class="tex-font-style-tt">+</span>'), and then the result of their addition, before which symbol'<span class="tex-font-style-tt">=</span>' should be. </p><p>Do not separate numbers and operation signs with spaces. Strictly follow the output format given in the examples.</p><p>If you remove symbol '<span class="tex-font-style-tt">+</span>' and symbol '<span class="tex-font-style-tt">=</span>' from answer string you should get a string, <span class="tex-font-style-bf">same as</span> string from the input data.</p></div>

## Input

<p>The first line contains a non-empty string consisting of digits. The length of the string does not exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p>

## Output

<p>Output the restored expression. If there are several solutions, you can print any of them.</p><p>Note that the answer <span class="tex-font-style-bf">at first</span> should contain two terms (divided with symbol '<span class="tex-font-style-tt">+</span>'), and then the result of their addition, before which symbol'<span class="tex-font-style-tt">=</span>' should be. </p><p>Do not separate numbers and operation signs with spaces. Strictly follow the output format given in the examples.</p><p>If you remove symbol '<span class="tex-font-style-tt">+</span>' and symbol '<span class="tex-font-style-tt">=</span>' from answer string you should get a string, <span class="tex-font-style-bf">same as</span> string from the input data.</p>





```input1
12345168

```




```input2
099

```




```input3
199100

```




```input4
123123123456456456579579579

```




```output1
123+45=168

```




```output2
0+9=9

```




```output3
1+99=100

```




```output4
123123123+456456456=579579579

```


