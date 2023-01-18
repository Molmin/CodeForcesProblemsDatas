## Description

<div><p>A string <span class="tex-span"><i>t</i></span> is called an <span class="tex-font-style-it">anagram</span> of the string <span class="tex-span"><i>s</i></span>, if it is possible to rearrange letters in <span class="tex-span"><i>t</i></span> so that it is identical to the string <span class="tex-span"><i>s</i></span>. For example, the string "<span class="tex-font-style-tt">aab</span>" is an anagram of the string "<span class="tex-font-style-tt">aba</span>" and the string "<span class="tex-font-style-tt">aaa</span>" is not.</p><p>The string <span class="tex-span"><i>t</i></span> is called a <span class="tex-font-style-it">substring</span> of the string <span class="tex-span"><i>s</i></span> if it can be read starting from some position in the string <span class="tex-span"><i>s</i></span>. For example, the string "<span class="tex-font-style-tt">aba</span>" has six substrings: "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>", "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">ab</span>", "<span class="tex-font-style-tt">ba</span>", "<span class="tex-font-style-tt">aba</span>".</p><p>You are given a string <span class="tex-span"><i>s</i></span>, consisting of lowercase Latin letters and characters "<span class="tex-font-style-tt">?</span>". You are also given a string <span class="tex-span"><i>p</i></span>, consisting of lowercase Latin letters only. Let's assume that a string is <span class="tex-font-style-it">good</span> if you can obtain an anagram of the string <span class="tex-span"><i>p</i></span> from it, replacing the "<span class="tex-font-style-tt">?</span>" characters by Latin letters. Each "<span class="tex-font-style-tt">?</span>" can be replaced by exactly one character of the Latin alphabet. For example, if the string <span class="tex-span"><i>p</i></span> = «<span class="tex-font-style-tt">aba</span>», then the string "<span class="tex-font-style-tt">a??</span>" is good, and the string «<span class="tex-font-style-tt">?bc</span>» is not. </p><p>Your task is to find the number of good substrings of the string <span class="tex-span"><i>s</i></span> (identical substrings must be counted in the answer several times).</p></div><div class="input-specification"><p>The first line is non-empty string <span class="tex-span"><i>s</i></span>, consisting of no more than <span class="tex-span">10<sup class="upper-index">5</sup></span> lowercase Latin letters and characters "<span class="tex-font-style-tt">?</span>". The second line is non-empty string <span class="tex-span"><i>p</i></span>, consisting of no more than <span class="tex-span">10<sup class="upper-index">5</sup></span> lowercase Latin letters. Please note that the length of the string <span class="tex-span"><i>p</i></span> can exceed the length of the string <span class="tex-span"><i>s</i></span>.</p></div><div class="output-specification"><p>Print the single number representing the number of good substrings of string <span class="tex-span"><i>s</i></span>.</p><p>Two substrings are considered different in their positions of occurrence are different. Thus, if some string occurs several times, then it should be counted the same number of times.</p></div>

## Input

<p>The first line is non-empty string <span class="tex-span"><i>s</i></span>, consisting of no more than <span class="tex-span">10<sup class="upper-index">5</sup></span> lowercase Latin letters and characters "<span class="tex-font-style-tt">?</span>". The second line is non-empty string <span class="tex-span"><i>p</i></span>, consisting of no more than <span class="tex-span">10<sup class="upper-index">5</sup></span> lowercase Latin letters. Please note that the length of the string <span class="tex-span"><i>p</i></span> can exceed the length of the string <span class="tex-span"><i>s</i></span>.</p>

## Output

<p>Print the single number representing the number of good substrings of string <span class="tex-span"><i>s</i></span>.</p><p>Two substrings are considered different in their positions of occurrence are different. Thus, if some string occurs several times, then it should be counted the same number of times.</p>





```input1
bb??x???
aab

```




```input2
ab?c
acb

```




```output1
2

```




```output2
2

```



## Note

<p>Consider the first sample test. Here the string <span class="tex-span"><i>s</i></span> has two good substrings: "<span class="tex-font-style-tt">b??</span>" (after we replace the question marks we get "<span class="tex-font-style-tt">baa</span>"), "<span class="tex-font-style-tt">???</span>" (after we replace the question marks we get "<span class="tex-font-style-tt">baa</span>").</p><p>Let's consider the second sample test. Here the string <span class="tex-span"><i>s</i></span> has two good substrings: "<span class="tex-font-style-tt">ab?</span>" ("<span class="tex-font-style-tt">?</span>" can be replaced by "<span class="tex-font-style-tt">c</span>"), "<span class="tex-font-style-tt">b?c</span>" ("<span class="tex-font-style-tt">?</span>" can be replaced by "<span class="tex-font-style-tt">a</span>").</p>
