## Description

<div><p>Little Petya loves presents. His mum bought him two strings of the same size for his birthday. The strings consist of uppercase and lowercase Latin letters. Now Petya wants to compare those two strings <span class="tex-font-style-underline">lexicographically</span>. The letters' case does not matter, that is an uppercase letter is considered equivalent to the corresponding lowercase letter. Help Petya perform the comparison.</p></div><div class="input-specification"><p>Each of the first two lines contains a bought string. The strings' lengths range from <span class="tex-span">1</span> to <span class="tex-span">100</span> inclusive. It is guaranteed that the strings are of the same length and also consist of uppercase and lowercase Latin letters.</p></div><div class="output-specification"><p>If the first string is less than the second one, print "-1". If the second string is less than the first one, print "1". If the strings are equal, print "0". Note that the letters' case is not taken into consideration when the strings are compared.</p></div>

## Input

<p>Each of the first two lines contains a bought string. The strings' lengths range from <span class="tex-span">1</span> to <span class="tex-span">100</span> inclusive. It is guaranteed that the strings are of the same length and also consist of uppercase and lowercase Latin letters.</p>

## Output

<p>If the first string is less than the second one, print "-1". If the second string is less than the first one, print "1". If the strings are equal, print "0". Note that the letters' case is not taken into consideration when the strings are compared.</p>





```input1
aaaa
aaaA

```




```input2
abs
Abz

```




```input3
abcdefg
AbCdEfF

```




```output1
0

```




```output2
-1

```




```output3
1

```



## Note

<p>If you want more formal information about the lexicographical order (also known as the "<span class="tex-font-style-underline">dictionary order</span>" or "<span class="tex-font-style-underline">alphabetical order</span>"), you can visit the following site:</p><ul><li> <span class="tex-font-style-tt">http://en.wikipedia.org/wiki/Lexicographical_order</span></li></ul>
