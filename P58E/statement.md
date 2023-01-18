## Description

<div><p>One day Vasya was solving arithmetical problems. He wrote down an expression <span class="tex-span"><i>a</i> + <i>b</i> = <i>c</i></span> in his notebook. When the teacher checked Vasya's work it turned out that Vasya had solved the problem incorrectly. Now Vasya tries to find excuses. He says that he simply forgot to write down several digits in numbers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span>, but he can't remember what numbers they actually were. Help Vasya, find such numbers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>z</i></span>, with which the following conditions are met: </p><ul> <li> <span class="tex-span"><i>x</i> + <i>y</i> = <i>z</i></span>, </li><li> from the expression <span class="tex-span"><i>x</i> + <i>y</i> = <i>z</i></span> several digits can be erased in such a way that the result will be <span class="tex-span"><i>a</i> + <i>b</i> = <i>c</i></span>, </li><li> the expression <span class="tex-span"><i>x</i> + <i>y</i> = <i>z</i></span> should have the minimal length. </li></ul></div><div class="input-specification"><p>The first and only input line contains the expression <span class="tex-span"><i>a</i> + <i>b</i> = <i>c</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>c</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> don't contain leading zeroes) which is the expression Vasya wrote down.</p></div><div class="output-specification"><p>Print the correct expression <span class="tex-span"><i>x</i> + <i>y</i> = <i>z</i></span> (<span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>z</i></span> are non-negative numbers without leading zeroes). The expression <span class="tex-span"><i>a</i> + <i>b</i> = <i>c</i></span> must be met in <span class="tex-span"><i>x</i> + <i>y</i> = <i>z</i></span> as a subsequence. The printed solution should have the minimal possible number of characters. If there are several such solutions, you can print any of them.</p></div>

## Input

<p>The first and only input line contains the expression <span class="tex-span"><i>a</i> + <i>b</i> = <i>c</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>c</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> don't contain leading zeroes) which is the expression Vasya wrote down.</p>

## Output

<p>Print the correct expression <span class="tex-span"><i>x</i> + <i>y</i> = <i>z</i></span> (<span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>z</i></span> are non-negative numbers without leading zeroes). The expression <span class="tex-span"><i>a</i> + <i>b</i> = <i>c</i></span> must be met in <span class="tex-span"><i>x</i> + <i>y</i> = <i>z</i></span> as a subsequence. The printed solution should have the minimal possible number of characters. If there are several such solutions, you can print any of them.</p>





```input1
2+4=5

```




```input2
1+1=3

```




```input3
1+1=2

```




```output1
21+4=25

```




```output2
1+31=32

```




```output3
1+1=2

```


