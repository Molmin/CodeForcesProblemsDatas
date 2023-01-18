## Description

<div><p>You are given a string <span class="tex-span"><i>s</i></span> consisting of <span class="tex-span">|<i>s</i>|</span> small english letters.</p><p>In one move you can replace any character of this string to the next character in alphabetical order (<span class="tex-font-style-tt">a</span> will be replaced with <span class="tex-font-style-tt">b</span>, <span class="tex-font-style-tt">s</span> will be replaced with <span class="tex-font-style-tt">t</span>, etc.). You cannot replace letter <span class="tex-font-style-tt">z</span> with any other letter.</p><p>Your target is to make some number of moves (not necessary minimal) to get string <span class="tex-font-style-tt">abcdefghijklmnopqrstuvwxyz</span> (english alphabet) as a subsequence. Subsequence of the string is the string that is obtained by deleting characters at some positions. You need to print the string that will be obtained from the given string and will be contain english alphabet as a subsequence or say that it is impossible.</p></div><div class="input-specification"><p>The only one line of the input consisting of the string <span class="tex-span"><i>s</i></span> consisting of <span class="tex-span">|<i>s</i>|</span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">5</sup></span>) small english letters.</p></div><div class="output-specification"><p>If you can get a string that can be obtained from the given string and will contain english alphabet as a subsequence, print it. Otherwise print «-1» (without quotes).</p></div>

## Input

<p>The only one line of the input consisting of the string <span class="tex-span"><i>s</i></span> consisting of <span class="tex-span">|<i>s</i>|</span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">5</sup></span>) small english letters.</p>

## Output

<p>If you can get a string that can be obtained from the given string and will contain english alphabet as a subsequence, print it. Otherwise print «-1» (without quotes).</p>





```input1
aacceeggiikkmmooqqssuuwwyy

```




```input2
thereisnoanswer

```




```output1
abcdefghijklmnopqrstuvwxyz

```




```output2
-1

```


