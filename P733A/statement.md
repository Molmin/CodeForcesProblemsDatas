## Description

<div><p>One day, the Grasshopper was jumping on the lawn and found a piece of paper with a string. Grasshopper became interested what is the minimum <span class="tex-font-style-it">jump ability</span> he should have in order to be able to reach the far end of the string, jumping only on vowels of the English alphabet. <span class="tex-font-style-it">Jump ability</span> is the maximum possible length of his jump. </p><p>Formally, consider that at the begginning the Grasshopper is located directly in front of the leftmost character of the string. His goal is to reach the position right after the rightmost character of the string. In one jump the Grasshopper could jump to the right any distance from <span class="tex-span">1</span> to the value of his <span class="tex-font-style-it">jump ability</span>.</p><center> <img class="tex-graphics" src="file://TKURBpZT.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">The picture corresponds to the first example.</span> </center><p>The following letters are vowels: '<span class="tex-font-style-tt">A</span>', '<span class="tex-font-style-tt">E</span>', '<span class="tex-font-style-tt">I</span>', '<span class="tex-font-style-tt">O</span>', '<span class="tex-font-style-tt">U</span>' and '<span class="tex-font-style-tt">Y</span>'.</p></div><div class="input-specification"><p>The first line contains non-empty string consisting of capital English letters. It is guaranteed that the length of the string does not exceed 100. </p></div><div class="output-specification"><p>Print single integer <span class="tex-span"><i>a</i></span>&nbsp;— the minimum <span class="tex-font-style-it">jump ability</span> of the Grasshopper (in the number of symbols) that is needed to overcome the given string, jumping only on vowels.</p></div>

## Input

<p>The first line contains non-empty string consisting of capital English letters. It is guaranteed that the length of the string does not exceed 100. </p>

## Output

<p>Print single integer <span class="tex-span"><i>a</i></span>&nbsp;— the minimum <span class="tex-font-style-it">jump ability</span> of the Grasshopper (in the number of symbols) that is needed to overcome the given string, jumping only on vowels.</p>





```input1
ABABBBACFEYUKOTT

```




```input2
AAA

```




```output1
4
```




```output2
1
```


