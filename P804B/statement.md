## Description

<div><p>We have a string of letters '<span class="tex-font-style-tt">a</span>' and '<span class="tex-font-style-tt">b</span>'. We want to perform some operations on it. On each step we choose one of substrings "<span class="tex-font-style-tt">ab</span>" in the string and replace it with the string "<span class="tex-font-style-tt">bba</span>". If we have no "<span class="tex-font-style-tt">ab</span>" as a substring, our job is done. Print the minimum number of steps we should perform to make our job done modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p><p>The string "<span class="tex-font-style-tt">ab</span>" appears as a substring if there is a letter '<span class="tex-font-style-tt">b</span>' right after the letter '<span class="tex-font-style-tt">a</span>' somewhere in the string.</p></div><div class="input-specification"><p>The first line contains the initial string consisting of letters '<span class="tex-font-style-tt">a</span>' and '<span class="tex-font-style-tt">b</span>' only with length from <span class="tex-span">1</span> to <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p></div><div class="output-specification"><p>Print the minimum number of steps modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line contains the initial string consisting of letters '<span class="tex-font-style-tt">a</span>' and '<span class="tex-font-style-tt">b</span>' only with length from <span class="tex-span">1</span> to <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p>

## Output

<p>Print the minimum number of steps modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
ab

```




```input2
aab

```




```output1
1

```




```output2
3

```



## Note

<p>The first example: "<span class="tex-font-style-tt">ab</span>" <span class="tex-span"> → </span> "<span class="tex-font-style-tt">bba</span>".</p><p>The second example: "<span class="tex-font-style-tt">aab</span>" <span class="tex-span"> → </span> "<span class="tex-font-style-tt">abba</span>" <span class="tex-span"> → </span> "<span class="tex-font-style-tt">bbaba</span>" <span class="tex-span"> → </span> "<span class="tex-font-style-tt">bbbbaa</span>".</p>
