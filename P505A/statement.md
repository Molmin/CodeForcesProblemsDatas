## Description

<div><p>Mr. Kitayuta has kindly given you a string <span class="tex-span"><i>s</i></span> consisting of lowercase English letters. You are asked to insert exactly one lowercase English letter into <span class="tex-span"><i>s</i></span> to make it a palindrome. A <span class="tex-font-style-it">palindrome</span> is a string that reads the same forward and backward. For example, "<span class="tex-font-style-tt">noon</span>", "<span class="tex-font-style-tt">testset</span>" and "<span class="tex-font-style-tt">a</span>" are all palindromes, while "<span class="tex-font-style-tt">test</span>" and "<span class="tex-font-style-tt">kitayuta</span>" are not.</p><p>You can choose any lowercase English letter, and insert it to any position of <span class="tex-span"><i>s</i></span>, possibly to the beginning or the end of <span class="tex-span"><i>s</i></span>. You have to insert a letter even if the given string is already a palindrome.</p><p>If it is possible to insert one lowercase English letter into <span class="tex-span"><i>s</i></span> so that the resulting string will be a palindrome, print the string after the insertion. Otherwise, print "<span class="tex-font-style-tt">NA</span>" (without quotes, case-sensitive). In case there is more than one palindrome that can be obtained, you are allowed to print any of them.</p></div><div class="input-specification"><p>The only line of the input contains a string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 10</span>). Each character in <span class="tex-span"><i>s</i></span> is a lowercase English letter.</p></div><div class="output-specification"><p>If it is possible to turn <span class="tex-span"><i>s</i></span> into a palindrome by inserting one lowercase English letter, print the resulting string in a single line. Otherwise, print "<span class="tex-font-style-tt">NA</span>" (without quotes, case-sensitive). In case there is more than one solution, any of them will be accepted. </p></div>

## Input

<p>The only line of the input contains a string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 10</span>). Each character in <span class="tex-span"><i>s</i></span> is a lowercase English letter.</p>

## Output

<p>If it is possible to turn <span class="tex-span"><i>s</i></span> into a palindrome by inserting one lowercase English letter, print the resulting string in a single line. Otherwise, print "<span class="tex-font-style-tt">NA</span>" (without quotes, case-sensitive). In case there is more than one solution, any of them will be accepted. </p>





```input1
revive

```




```input2
ee

```




```input3
kitayuta

```




```output1
reviver

```




```output2
eye
```




```output3
NA

```



## Note

<p>For the first sample, insert '<span class="tex-font-style-tt">r</span>' to the end of "<span class="tex-font-style-tt">revive</span>" to obtain a palindrome "<span class="tex-font-style-tt">reviver</span>".</p><p>For the second sample, there is more than one solution. For example, "<span class="tex-font-style-tt">eve</span>" will also be accepted.</p><p>For the third sample, it is not possible to turn "<span class="tex-font-style-tt">kitayuta</span>" into a palindrome by just inserting one letter.</p>
