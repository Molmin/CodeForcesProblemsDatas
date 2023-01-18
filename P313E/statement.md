## Description

<div><p>Ilya has recently taken up archaeology. He's recently found two numbers, written in the <span class="tex-span"><i>m</i></span>-based notation. Each of the found numbers consisted of exactly <span class="tex-span"><i>n</i></span> digits. Ilya immediately started looking for information about those numbers. He learned that the numbers are part of a cyphered code and the one who can decypher it can get the greatest treasure.</p><p>After considerable research Ilya understood that to decypher the code, he should do the following:</p><ul> <li> Rearrange digits in the first number in some manner. Similarly, rearrange digits in the second number in some manner. As a result of this operation, the numbers can get leading zeroes. </li><li> Add numbers, digit by digit, modulo <span class="tex-span"><i>m</i></span>. In other words, we need to get the third number of length <span class="tex-span"><i>n</i></span>, each digit of the number is the sum of the respective numbers of the found numbers. For example, suppose there are two numbers recorded in the ternary notation, 001210 and 012111, then if you add them to each other digit by digit modulo 3, you will get number 010021. </li><li> The key to the code is the maximum possible number that can be obtained in the previous step. </li></ul><p>Help Ilya, find the key to the code.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>, <i>m</i> &gt; 1)</span>. The second line contains the first found number, the third line contains the second found number. </p><p>The numbers are recorded as a sequence of digits in the <span class="tex-span"><i>m</i></span>-based notation. Each digit is an integer from 0 to <span class="tex-span"><i>m</i> - 1</span>. The digits in the line are written in the order from the most significant digits to the least significant ones.</p><p>The given numbers can contain leading zeroes.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> <span class="tex-span"><i>m</i></span>-base digits. The resulting third number written in the <span class="tex-span"><i>m</i></span>-based notation. Print the digits in the order from the most significant digits to the least significant ones.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>, <i>m</i> &gt; 1)</span>. The second line contains the first found number, the third line contains the second found number. </p><p>The numbers are recorded as a sequence of digits in the <span class="tex-span"><i>m</i></span>-based notation. Each digit is an integer from 0 to <span class="tex-span"><i>m</i> - 1</span>. The digits in the line are written in the order from the most significant digits to the least significant ones.</p><p>The given numbers can contain leading zeroes.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> <span class="tex-span"><i>m</i></span>-base digits. The resulting third number written in the <span class="tex-span"><i>m</i></span>-based notation. Print the digits in the order from the most significant digits to the least significant ones.</p>





```input1
4 7
5 4 3 2
5 6 5 4

```




```input2
5 5
2 4 4 1 3
1 0 1 2 4

```




```output1
6 4 2 1 

```




```output2
4 4 4 3 2 

```


