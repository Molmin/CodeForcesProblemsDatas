## Description

<div><p>Tonio has a keyboard with only two letters, "<span class="tex-font-style-tt">V</span>" and "<span class="tex-font-style-tt">K</span>".</p><p>One day, he has typed out a string <span class="tex-span"><i>s</i></span> with only these two letters. He really likes it when the string "<span class="tex-font-style-tt">VK</span>" appears, so he wishes to change at most one letter in the string (or do no changes) to maximize the number of occurrences of that string. Compute the maximum number of times "<span class="tex-font-style-tt">VK</span>" can appear as a substring (i.&nbsp;e. a letter "<span class="tex-font-style-tt">K</span>" right after a letter "<span class="tex-font-style-tt">V</span>") in the resulting string.</p></div><div class="input-specification"><p>The first line will contain a string <span class="tex-span"><i>s</i></span> consisting only of uppercase English letters "<span class="tex-font-style-tt">V</span>" and "<span class="tex-font-style-tt">K</span>" with length not less than <span class="tex-span">1</span> and not greater than <span class="tex-span">100</span>.</p></div><div class="output-specification"><p>Output a single integer, the maximum number of times "<span class="tex-font-style-tt">VK</span>" can appear as a substring of the given string after changing at most one character.</p></div>

## Input

<p>The first line will contain a string <span class="tex-span"><i>s</i></span> consisting only of uppercase English letters "<span class="tex-font-style-tt">V</span>" and "<span class="tex-font-style-tt">K</span>" with length not less than <span class="tex-span">1</span> and not greater than <span class="tex-span">100</span>.</p>

## Output

<p>Output a single integer, the maximum number of times "<span class="tex-font-style-tt">VK</span>" can appear as a substring of the given string after changing at most one character.</p>





```input1
VK

```




```input2
VV

```




```input3
V

```




```input4
VKKKKKKKKKVVVVVVVVVK

```




```input5
KVKV

```




```output1
1

```




```output2
1

```




```output3
0

```




```output4
3

```




```output5
1

```



## Note

<p>For the first case, we do not change any letters. "<span class="tex-font-style-tt">VK</span>" appears once, which is the maximum number of times it could appear.</p><p>For the second case, we can change the second character from a "<span class="tex-font-style-tt">V</span>" to a "<span class="tex-font-style-tt">K</span>". This will give us the string "<span class="tex-font-style-tt">VK</span>". This has one occurrence of the string "<span class="tex-font-style-tt">VK</span>" as a substring.</p><p>For the fourth case, we can change the fourth character from a "<span class="tex-font-style-tt">K</span>" to a "<span class="tex-font-style-tt">V</span>". This will give us the string "<span class="tex-font-style-tt">VKKVKKKKKKVVVVVVVVVK</span>". This has three occurrences of the string "<span class="tex-font-style-tt">VK</span>" as a substring. We can check no other moves can give us strictly more occurrences.</p>
