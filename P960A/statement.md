## Description

<div><p>A has a string consisting of some number of lowercase English letters '<span class="tex-font-style-tt">a</span>'. He gives it to his friend B who appends some number of letters '<span class="tex-font-style-tt">b</span>' to the end of this string. Since both A and B like the characters '<span class="tex-font-style-tt">a</span>' and '<span class="tex-font-style-tt">b</span>', they have made sure that at this point, <span class="tex-font-style-bf">at least one '<span class="tex-font-style-tt">a</span>' and one '<span class="tex-font-style-tt">b</span>'</span> exist in the string.</p><p>B now gives this string to C and he appends some number of letters '<span class="tex-font-style-tt">c</span>' to the end of the string. However, since C is a good friend of A and B, the number of letters '<span class="tex-font-style-tt">c</span>' he appends is equal to the number of '<span class="tex-font-style-tt">a</span>' or to the number of '<span class="tex-font-style-tt">b</span>' in the string. It is also possible that the number of letters '<span class="tex-font-style-tt">c</span>' equals both to the number of letters '<span class="tex-font-style-tt">a</span>' and to the number of letters '<span class="tex-font-style-tt">b</span>' at the same time.</p><p>You have a string in your hands, and you want to check if it is possible to obtain the string in this way or not. If it is possible to obtain the string, print "<span class="tex-font-style-tt">YES</span>", otherwise print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p></div><div class="input-specification"><p>The first and only line consists of a string $S$ ($ 1 \le |S| \le 5\,000 $). It is guaranteed that the string will only consist of the lowercase English letters '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>', '<span class="tex-font-style-tt">c</span>'.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" or "<span class="tex-font-style-tt">NO</span>", according to the condition.</p></div>

## Input

<p>The first and only line consists of a string $S$ ($ 1 \le |S| \le 5\,000 $). It is guaranteed that the string will only consist of the lowercase English letters '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>', '<span class="tex-font-style-tt">c</span>'.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" or "<span class="tex-font-style-tt">NO</span>", according to the condition.</p>





```input1
aaabccc

```




```input2
bbacc

```




```input3
aabc

```




```output1
YES

```




```output2
NO

```




```output3
YES

```



## Note

<p>Consider first example: the number of '<span class="tex-font-style-tt">c</span>' is equal to the number of '<span class="tex-font-style-tt">a</span>'. </p><p>Consider second example: although the number of '<span class="tex-font-style-tt">c</span>' is equal to the number of the '<span class="tex-font-style-tt">b</span>', the order is not correct.</p><p>Consider third example: the number of '<span class="tex-font-style-tt">c</span>' is equal to the number of '<span class="tex-font-style-tt">b</span>'.</p>
