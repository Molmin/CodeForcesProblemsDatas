## Description

<div><p>You are given a non-negative integer <span class="tex-span"><i>n</i></span>, its decimal representation consists of at most <span class="tex-span">100</span> digits and doesn't contain leading zeroes.</p><p>Your task is to determine if it is possible in this case to remove some of the digits (possibly not remove any digit at all) so that the result contains at least one digit, forms a non-negative integer, doesn't have leading zeroes and is divisible by 8. After the removing, it is forbidden to rearrange the digits.</p><p>If a solution exists, you should print it.</p></div><div class="input-specification"><p>The single line of the input contains a non-negative integer <span class="tex-span"><i>n</i></span>. The representation of number <span class="tex-span"><i>n</i></span> doesn't contain any leading zeroes and its length doesn't exceed <span class="tex-span">100</span> digits. </p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">NO</span>" (without quotes), if there is no such way to remove some digits from number <span class="tex-span"><i>n</i></span>. </p><p>Otherwise, print "<span class="tex-font-style-tt">YES</span>" in the first line and the resulting number after removing digits from number <span class="tex-span"><i>n</i></span> in the second line. The printed number must be divisible by <span class="tex-span">8</span>.</p><p>If there are multiple possible answers, you may print any of them.</p></div>

## Input

<p>The single line of the input contains a non-negative integer <span class="tex-span"><i>n</i></span>. The representation of number <span class="tex-span"><i>n</i></span> doesn't contain any leading zeroes and its length doesn't exceed <span class="tex-span">100</span> digits. </p>

## Output

<p>Print "<span class="tex-font-style-tt">NO</span>" (without quotes), if there is no such way to remove some digits from number <span class="tex-span"><i>n</i></span>. </p><p>Otherwise, print "<span class="tex-font-style-tt">YES</span>" in the first line and the resulting number after removing digits from number <span class="tex-span"><i>n</i></span> in the second line. The printed number must be divisible by <span class="tex-span">8</span>.</p><p>If there are multiple possible answers, you may print any of them.</p>





```input1
3454

```




```input2
10

```




```input3
111111

```




```output1
YES
344

```




```output2
YES
0

```




```output3
NO

```


