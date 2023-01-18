## Description

<div><p>Little walrus Fangy loves math very much. That's why when he is bored he plays with a number performing some operations.</p><p>Fangy takes some positive integer <span class="tex-span"><i>x</i></span> and wants to get a number one from it. While <span class="tex-span"><i>x</i></span> is not equal to <span class="tex-span">1</span>, Fangy repeats the following action: if <span class="tex-span"><i>x</i></span> is odd, then he adds <span class="tex-span">1</span> to it, otherwise he divides <span class="tex-span"><i>x</i></span> by <span class="tex-span">2</span>. Fangy knows that for any positive integer number the process ends in finite time.</p><p>How many actions should Fangy perform to get a number one from number <span class="tex-span"><i>x</i></span>?</p></div><div class="input-specification"><p>The first line contains a positive integer <span class="tex-span"><i>x</i></span> in a <span class="tex-font-style-bf">binary system</span>. It is guaranteed that the first digit of <span class="tex-span"><i>x</i></span> is different from a zero and the number of its digits does not exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p></div><div class="output-specification"><p>Print the required number of actions.</p></div>

## Input

<p>The first line contains a positive integer <span class="tex-span"><i>x</i></span> in a <span class="tex-font-style-bf">binary system</span>. It is guaranteed that the first digit of <span class="tex-span"><i>x</i></span> is different from a zero and the number of its digits does not exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p>

## Output

<p>Print the required number of actions.</p>





```input1
1

```




```input2
1001001

```




```input3
101110

```




```output1
0

```




```output2
12

```




```output3
8

```



## Note

<p>Let's consider the third sample. Number <span class="tex-span">101110</span> is even, which means that we should divide it by <span class="tex-span">2</span>. After the dividing Fangy gets an odd number <span class="tex-span">10111</span> and adds one to it. Number <span class="tex-span">11000</span> can be divided by <span class="tex-span">2</span> three times in a row and get number <span class="tex-span">11</span>. All that's left is to increase the number by one (we get <span class="tex-span">100</span>), and then divide it by <span class="tex-span">2</span> two times in a row. As a result, we get <span class="tex-span">1</span>.</p>
