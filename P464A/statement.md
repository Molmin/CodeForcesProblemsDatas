## Description

<div><p>Paul <span class="tex-font-style-underline">hates</span> palindromes. He assumes that string <span class="tex-span"><i>s</i></span> is <span class="tex-font-style-underline">tolerable</span> if each its character is one of the first <span class="tex-span"><i>p</i></span> letters of the English alphabet and <span class="tex-span"><i>s</i></span> doesn't contain any palindrome contiguous substring of length 2 or more.</p><p>Paul has found a tolerable string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span>. Help him find the lexicographically next tolerable string of the same length or else state that such string does not exist.</p></div><div class="input-specification"><p>The first line contains two space-separated integers: <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>; <span class="tex-span">1 ≤ <i>p</i> ≤ 26</span>). The second line contains string <span class="tex-span"><i>s</i></span>, consisting of <span class="tex-span"><i>n</i></span> small English letters. It is guaranteed that the string is tolerable (according to the above definition).</p></div><div class="output-specification"><p>If the lexicographically next tolerable string of the same length exists, print it. Otherwise, print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p></div>

## Input

<p>The first line contains two space-separated integers: <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>; <span class="tex-span">1 ≤ <i>p</i> ≤ 26</span>). The second line contains string <span class="tex-span"><i>s</i></span>, consisting of <span class="tex-span"><i>n</i></span> small English letters. It is guaranteed that the string is tolerable (according to the above definition).</p>

## Output

<p>If the lexicographically next tolerable string of the same length exists, print it. Otherwise, print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p>





```input1
3 3
cba

```




```input2
3 4
cba

```




```input3
4 4
abcd

```




```output1
NO

```




```output2
cbd

```




```output3
abda

```



## Note

<p>String <span class="tex-span"><i>s</i></span> is <span class="tex-font-style-underline">lexicographically larger</span> (or simply <span class="tex-font-style-underline">larger</span>) than string <span class="tex-span"><i>t</i></span> with the same length, if there is number <span class="tex-span"><i>i</i></span>, such that <span class="tex-span"><i>s</i><sub class="lower-index">1</sub> = <i>t</i><sub class="lower-index">1</sub></span>, ..., <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> = <i>t</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i> + 1</sub> &gt; <i>t</i><sub class="lower-index"><i>i</i> + 1</sub></span>.</p><p>The lexicographically next tolerable string is the lexicographically minimum tolerable string which is larger than the given one.</p><p>A palindrome is a string that reads the same forward or reversed.</p>
