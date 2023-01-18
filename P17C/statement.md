## Description

<div><p>Nick likes strings very much, he likes to rotate them, sort them, rearrange characters within a string... Once he wrote a random string of characters <span class="tex-font-style-tt">a</span>, <span class="tex-font-style-tt">b</span>, <span class="tex-font-style-tt">c</span> on a piece of paper and began to perform the following operations: </p><ul> <li> to take two adjacent characters and replace the second character with the first one, </li><li> to take two adjacent characters and replace the first character with the second one </li></ul><p>To understand these actions better, let's take a look at a string «<span class="tex-font-style-tt">abc</span>». All of the following strings can be obtained by performing one of the described operations on «<span class="tex-font-style-tt">abc</span>»: «<span class="tex-font-style-tt">bbc</span>», «<span class="tex-font-style-tt">abb</span>», «<span class="tex-font-style-tt">acc</span>». Let's denote the <span class="tex-font-style-underline">frequency of a character</span> for each of the characters <span class="tex-font-style-tt">a</span>, <span class="tex-font-style-tt">b</span> and <span class="tex-font-style-tt">c</span> as the number of occurrences of this character in the string. For example, for string «<span class="tex-font-style-tt">abc</span>»: |<span class="tex-span"><i>a</i></span>| = 1, |<span class="tex-span"><i>b</i></span>| = 1, |<span class="tex-span"><i>c</i></span>| = 1, and for string «<span class="tex-font-style-tt">bbc</span>»: |<span class="tex-span"><i>a</i></span>| = 0, |<span class="tex-span"><i>b</i></span>| = 2, |<span class="tex-span"><i>c</i></span>| = 1. </p><p>While performing the described operations, Nick sometimes got <span class="tex-font-style-underline">balanced strings</span>. Let's say that a string is balanced, if the frequencies of each character differ by at most 1. That is <span class="tex-span"> - 1 ≤ |<i>a</i>| - |<i>b</i>| ≤ 1</span>, <span class="tex-span"> - 1 ≤ |<i>a</i>| - |<i>c</i>| ≤ 1</span> и <span class="tex-span"> - 1 ≤ |<i>b</i>| - |<i>c</i>| ≤ 1</span>. </p><p>Would you help Nick find the number of different balanced strings that can be obtained by performing the operations described above, perhaps multiple times, on the given string <span class="tex-span"><i>s</i></span>. This number should be calculated modulo <span class="tex-span">51123987</span>.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 150</span>) — the length of the given string <span class="tex-span"><i>s</i></span>. Next line contains the given string <span class="tex-span"><i>s</i></span>. The initial string can be balanced as well, in this case it should be counted too. The given string <span class="tex-span"><i>s</i></span> consists only of characters <span class="tex-font-style-tt">a</span>, <span class="tex-font-style-tt">b</span> and <span class="tex-font-style-tt">c</span>.</p></div><div class="output-specification"><p>Output the only number — the number of different balanced strings that can be obtained by performing the described operations, perhaps multiple times, on the given string <span class="tex-span"><i>s</i></span>, modulo <span class="tex-span">51123987</span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 150</span>) — the length of the given string <span class="tex-span"><i>s</i></span>. Next line contains the given string <span class="tex-span"><i>s</i></span>. The initial string can be balanced as well, in this case it should be counted too. The given string <span class="tex-span"><i>s</i></span> consists only of characters <span class="tex-font-style-tt">a</span>, <span class="tex-font-style-tt">b</span> and <span class="tex-font-style-tt">c</span>.</p>

## Output

<p>Output the only number — the number of different balanced strings that can be obtained by performing the described operations, perhaps multiple times, on the given string <span class="tex-span"><i>s</i></span>, modulo <span class="tex-span">51123987</span>.</p>





```input1
4
abca

```




```input2
4
abbc

```




```input3
2
ab

```




```output1
7

```




```output2
3

```




```output3
1

```



## Note

<p>In the first sample it is possible to get <span class="tex-span">51</span> different strings through the described operations, but only <span class="tex-span">7</span> of them are balanced: «<span class="tex-font-style-tt">abca</span>», «<span class="tex-font-style-tt">bbca</span>», «<span class="tex-font-style-tt">bcca</span>», «<span class="tex-font-style-tt">bcaa</span>», «<span class="tex-font-style-tt">abcc</span>», «<span class="tex-font-style-tt">abbc</span>», «<span class="tex-font-style-tt">aabc</span>». In the second sample: «<span class="tex-font-style-tt">abbc</span>», «<span class="tex-font-style-tt">aabc</span>», «<span class="tex-font-style-tt">abcc</span>». In the third sample there is only one balanced string — «<span class="tex-font-style-tt">ab</span>» itself.</p>
