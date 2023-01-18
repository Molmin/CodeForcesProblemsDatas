## Description

<div><p>Kolya has a string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span> consisting of lowercase and uppercase Latin letters and digits.</p><p>He wants to rearrange the symbols in <span class="tex-span"><i>s</i></span> and cut it into the minimum number of parts so that each part is a palindrome and all parts have <span class="tex-font-style-it">the same lengths</span>. A palindrome is a string which reads the same backward as forward, such as <span class="tex-font-style-tt">madam</span> or <span class="tex-font-style-tt">racecar</span>.</p><p>Your task is to help Kolya and determine the minimum number of palindromes of equal lengths to cut <span class="tex-span"><i>s</i></span> into, if it is allowed to rearrange letters in <span class="tex-span"><i>s</i></span> before cuttings.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 4·10<sup class="upper-index">5</sup></span>) — the length of string <span class="tex-span"><i>s</i></span>.</p><p>The second line contains a string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span> consisting of lowercase and uppercase Latin letters and digits.</p></div><div class="output-specification"><p>Print to the first line an integer <span class="tex-span"><i>k</i></span> — minimum number of palindromes into which you can cut a given string.</p><p>Print to the second line <span class="tex-span"><i>k</i></span> strings — the palindromes themselves. Separate them by a space. You are allowed to print palindromes in arbitrary order. All of them should have the same length.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 4·10<sup class="upper-index">5</sup></span>) — the length of string <span class="tex-span"><i>s</i></span>.</p><p>The second line contains a string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span> consisting of lowercase and uppercase Latin letters and digits.</p>

## Output

<p>Print to the first line an integer <span class="tex-span"><i>k</i></span> — minimum number of palindromes into which you can cut a given string.</p><p>Print to the second line <span class="tex-span"><i>k</i></span> strings — the palindromes themselves. Separate them by a space. You are allowed to print palindromes in arbitrary order. All of them should have the same length.</p>





```input1
6
aabaac

```




```input2
8
0rTrT022

```




```input3
2
aA

```




```output1
2
aba aca
```




```output2
1
02TrrT20
```




```output3
2
a A 

```


