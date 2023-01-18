## Description

<div><p>A substring of some string is called the most frequent, if the number of its occurrences is not less than number of occurrences of any other substring.</p><p>You are given a set of strings. A string (not necessarily from this set) is called good if all elements of the set are the most frequent substrings of this string. Restore the non-empty good string with minimum length. If several such strings exist, restore lexicographically minimum string. If there are no good strings, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>A substring of a string is a contiguous subsequence of letters in the string. For example, "<span class="tex-font-style-tt">ab</span>", "<span class="tex-font-style-tt">c</span>", "<span class="tex-font-style-tt">abc</span>" are substrings of string "<span class="tex-font-style-tt">abc</span>", while "<span class="tex-font-style-tt">ac</span>" is not a substring of that string.</p><p>The number of occurrences of a substring in a string is the number of starting positions in the string where the substring occurs. These occurrences could overlap.</p><p>String <span class="tex-span"><i>a</i></span> is lexicographically smaller than string <span class="tex-span"><i>b</i></span>, if <span class="tex-span"><i>a</i></span> is a prefix of <span class="tex-span"><i>b</i></span>, or <span class="tex-span"><i>a</i></span> has a smaller letter at the first position where <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> differ.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of strings in the set.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains a non-empty string consisting of lowercase English letters. It is guaranteed that the strings are distinct.</p><p>The total length of the strings doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p></div><div class="output-specification"><p>Print the non-empty good string with minimum length. If several good strings exist, print lexicographically minimum among them. Print "<span class="tex-font-style-tt">NO</span>" (without quotes) if there are no good strings.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of strings in the set.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains a non-empty string consisting of lowercase English letters. It is guaranteed that the strings are distinct.</p><p>The total length of the strings doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p>

## Output

<p>Print the non-empty good string with minimum length. If several good strings exist, print lexicographically minimum among them. Print "<span class="tex-font-style-tt">NO</span>" (without quotes) if there are no good strings.</p>





```input1
4
mail
ai
lru
cf

```




```input2
3
kek
preceq
cheburek

```




```output1
cfmailru

```




```output2
NO

```



## Note

<p>One can show that in the first sample only two good strings with minimum length exist: "<span class="tex-font-style-tt">cfmailru</span>" and "<span class="tex-font-style-tt">mailrucf</span>". The first string is lexicographically minimum.</p>
