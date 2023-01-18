## Description

<div><p>Copying large hexadecimal (base 16) strings by hand can be error prone, but that doesn't stop people from doing it. You've discovered a bug in the code that was likely caused by someone making a mistake when copying such a string. You suspect that whoever copied the string did not change any of the digits in the string, nor the length of the string, but may have permuted the digits arbitrarily. For example, if the original string was <span class="tex-span">0<i>abc</i></span> they may have changed it to <span class="tex-span"><i>a</i>0<i>cb</i></span> or <span class="tex-span">0<i>bca</i></span>, but not <span class="tex-span"><i>abc</i></span> or <span class="tex-span">0<i>abb</i></span>.</p><p>Unfortunately you don't have access to the original string nor the copied string, but you do know the length of the strings and their numerical absolute difference. You will be given this difference as a hexadecimal string <span class="tex-span"><i>S</i></span>, which has been zero-extended to be equal in length to the original and copied strings. Determine the smallest possible numerical value of the original string.</p></div><div class="input-specification"><p>Input will contain a hexadecimal string <span class="tex-span"><i>S</i></span> consisting only of digits <span class="tex-span">0</span> to <span class="tex-span">9</span> and lowercase English letters from <span class="tex-span"><i>a</i></span> to <span class="tex-span"><i>f</i></span>, with length at most <span class="tex-span">14</span>. At least one of the characters is non-zero.</p></div><div class="output-specification"><p>If it is not possible, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>Otherwise, print the lowercase hexadecimal string corresponding to the smallest possible numerical value, including any necessary leading zeros for the length to be correct.</p></div>

## Input

<p>Input will contain a hexadecimal string <span class="tex-span"><i>S</i></span> consisting only of digits <span class="tex-span">0</span> to <span class="tex-span">9</span> and lowercase English letters from <span class="tex-span"><i>a</i></span> to <span class="tex-span"><i>f</i></span>, with length at most <span class="tex-span">14</span>. At least one of the characters is non-zero.</p>

## Output

<p>If it is not possible, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>Otherwise, print the lowercase hexadecimal string corresponding to the smallest possible numerical value, including any necessary leading zeros for the length to be correct.</p>





```input1
f1e

```




```input2
0f1e

```




```input3
12d2c

```




```output1
NO

```




```output2
00f1

```




```output3
00314

```



## Note

<p>The numerical value of a hexadecimal string is computed by multiplying each digit by successive powers of <span class="tex-span">16</span>, starting with the rightmost digit, which is multiplied by <span class="tex-span">16<sup class="upper-index">0</sup></span>. Hexadecimal digits representing values greater than <span class="tex-span">9</span> are represented by letters: <span class="tex-span"><i>a</i> = 10, <i>b</i> = 11, <i>c</i> = 12, <i>d</i> = 13, <i>e</i> = 14, <i>f</i> = 15</span>.</p><p>For example, the numerical value of <span class="tex-span">0<i>f</i>1<i>e</i></span> is <span class="tex-span">0·16<sup class="upper-index">3</sup> + 15·16<sup class="upper-index">2</sup> + 1·16<sup class="upper-index">1</sup> + 14·16<sup class="upper-index">0</sup> = 3870</span>, the numerical value of <span class="tex-span">00<i>f</i>1</span> is <span class="tex-span">0·16<sup class="upper-index">3</sup> + 0·16<sup class="upper-index">2</sup> + 15·16<sup class="upper-index">1</sup> + 1·16<sup class="upper-index">0</sup> = 241</span>, and the numerical value of <span class="tex-span">100<i>f</i></span> is <span class="tex-span">1·16<sup class="upper-index">3</sup> + 0·16<sup class="upper-index">2</sup> + 0·16<sup class="upper-index">1</sup> + 15·16<sup class="upper-index">0</sup> = 4111</span>. Since <span class="tex-span">3870 + 241 = 4111</span> and <span class="tex-span">00<i>f</i>1</span> is a permutation of <span class="tex-span">100<i>f</i></span>, <span class="tex-span">00<i>f</i>1</span> is a valid answer to the second test case.</p>
