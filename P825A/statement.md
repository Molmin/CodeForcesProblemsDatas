## Description

<div><p>Polycarp has just invented a new binary protocol for data transmission. He is encoding positive integer decimal number to binary string using following algorithm:</p><ul> <li> Each digit is represented with number of <span class="tex-font-style-tt">'1'</span> characters equal to the value of that digit (for <span class="tex-font-style-tt">0</span> it is zero ones). </li><li> Digits are written one by one in order corresponding to number and separated by single <span class="tex-font-style-tt">'0'</span> character. </li></ul><p>Though Polycarp learnt how to encode the numbers, he has no idea how to decode them back. Help him calculate the decoded number.</p></div><div class="input-specification"><p>The first line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 89</span>) — length of the string <span class="tex-span"><i>s</i></span>.</p><p>The second line contains string <span class="tex-span"><i>s</i></span> — sequence of <span class="tex-font-style-tt">'0'</span> and <span class="tex-font-style-tt">'1'</span> characters, number in its encoded format. It is guaranteed that the number corresponding to the string is positive and doesn't exceed <span class="tex-span">10<sup class="upper-index">9</sup></span>. The string always starts with <span class="tex-font-style-tt">'1'</span>.</p></div><div class="output-specification"><p>Print the decoded number.</p></div>

## Input

<p>The first line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 89</span>) — length of the string <span class="tex-span"><i>s</i></span>.</p><p>The second line contains string <span class="tex-span"><i>s</i></span> — sequence of <span class="tex-font-style-tt">'0'</span> and <span class="tex-font-style-tt">'1'</span> characters, number in its encoded format. It is guaranteed that the number corresponding to the string is positive and doesn't exceed <span class="tex-span">10<sup class="upper-index">9</sup></span>. The string always starts with <span class="tex-font-style-tt">'1'</span>.</p>

## Output

<p>Print the decoded number.</p>





```input1
3
111

```




```input2
9
110011101

```




```output1
3

```




```output2
2031

```


