## Description

<div><p>You are given a rebus of form <span class="tex-font-style-tt">? + ? - ? + ? = n</span>, consisting of only question marks, separated by arithmetic operation '<span class="tex-font-style-tt">+</span>' and '<span class="tex-font-style-tt">-</span>', equality and positive integer <span class="tex-span"><i>n</i></span>. The goal is to replace each question mark with some positive integer from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, such that equality holds.</p></div><div class="input-specification"><p>The only line of the input contains a rebus. It's guaranteed that it contains no more than <span class="tex-span">100</span> question marks, integer <span class="tex-span"><i>n</i></span> is positive and doesn't exceed <span class="tex-span">1 000 000</span>, all letters and integers are separated by spaces, arithmetic operations are located only between question marks.</p></div><div class="output-specification"><p>The first line of the output should contain "<span class="tex-font-style-tt">Possible</span>" (without quotes) if rebus has a solution and "<span class="tex-font-style-tt">Impossible</span>" (without quotes) otherwise.</p><p>If the answer exists, the second line should contain any valid rebus with question marks replaced by integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Follow the format given in the samples.</p></div>

## Input

<p>The only line of the input contains a rebus. It's guaranteed that it contains no more than <span class="tex-span">100</span> question marks, integer <span class="tex-span"><i>n</i></span> is positive and doesn't exceed <span class="tex-span">1 000 000</span>, all letters and integers are separated by spaces, arithmetic operations are located only between question marks.</p>

## Output

<p>The first line of the output should contain "<span class="tex-font-style-tt">Possible</span>" (without quotes) if rebus has a solution and "<span class="tex-font-style-tt">Impossible</span>" (without quotes) otherwise.</p><p>If the answer exists, the second line should contain any valid rebus with question marks replaced by integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Follow the format given in the samples.</p>





```input1
? + ? - ? + ? + ? = 42

```




```input2
? - ? = 1

```




```input3
? = 1000000

```




```output1
Possible
9 + 13 - 39 + 28 + 31 = 42

```




```output2
Impossible

```




```output3
Possible
1000000 = 1000000

```


