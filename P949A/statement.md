## Description

<div><p>Oleg writes down the history of the days he lived. For each day he decides if it was good or bad. Oleg calls a non-empty sequence of days a <span class="tex-font-style-it">zebra</span>, if it starts with a bad day, ends with a bad day, and good and bad days are alternating in it. Let us denote bad days as <span class="tex-font-style-tt">0</span> and good days as <span class="tex-font-style-tt">1</span>. Then, for example, sequences of days <span class="tex-font-style-tt">0</span>, <span class="tex-font-style-tt">010</span>, <span class="tex-font-style-tt">01010</span> are zebras, while sequences <span class="tex-font-style-tt">1</span>, <span class="tex-font-style-tt">0110</span>, <span class="tex-font-style-tt">0101</span> are not.</p><p>Oleg tells you the story of days he lived in chronological order in form of string consisting of <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>. Now you are interested if it is possible to divide Oleg's life history into several <span class="tex-font-style-bf">subsequences</span>, each of which is a zebra, and the way it can be done. Each day must belong to exactly one of the subsequences. For each of the subsequences, days forming it must be ordered chronologically. Note that subsequence does not have to be a group of consecutive days. </p></div><div class="input-specification"><p>In the only line of input data there is a non-empty string <span class="tex-span"><i>s</i></span> consisting of characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>, which describes the history of Oleg's life. Its length (denoted as <span class="tex-span">|<i>s</i>|</span>) does not exceed <span class="tex-span">200 000</span> characters.</p></div><div class="output-specification"><p>If there is a way to divide history into zebra subsequences, in the first line of output you should print an integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ |<i>s</i>|</span>), the resulting number of subsequences. In the <span class="tex-span"><i>i</i></span>-th of following <span class="tex-span"><i>k</i></span> lines first print the integer <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ |<i>s</i>|</span>), which is the length of the <span class="tex-span"><i>i</i></span>-th subsequence, and then <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> indices of days forming the subsequence. Indices must follow in ascending order. Days are numbered starting from 1. Each index from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> must belong to exactly one subsequence. If there is no way to divide day history into zebra subsequences, print <span class="tex-font-style-tt">-1</span>.</p><p>Subsequences may be printed in any order. If there are several solutions, you may print any of them. You do not have to minimize nor maximize the value of <span class="tex-span"><i>k</i></span>.</p></div>

## Input

<p>In the only line of input data there is a non-empty string <span class="tex-span"><i>s</i></span> consisting of characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>, which describes the history of Oleg's life. Its length (denoted as <span class="tex-span">|<i>s</i>|</span>) does not exceed <span class="tex-span">200 000</span> characters.</p>

## Output

<p>If there is a way to divide history into zebra subsequences, in the first line of output you should print an integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ |<i>s</i>|</span>), the resulting number of subsequences. In the <span class="tex-span"><i>i</i></span>-th of following <span class="tex-span"><i>k</i></span> lines first print the integer <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ |<i>s</i>|</span>), which is the length of the <span class="tex-span"><i>i</i></span>-th subsequence, and then <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> indices of days forming the subsequence. Indices must follow in ascending order. Days are numbered starting from 1. Each index from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> must belong to exactly one subsequence. If there is no way to divide day history into zebra subsequences, print <span class="tex-font-style-tt">-1</span>.</p><p>Subsequences may be printed in any order. If there are several solutions, you may print any of them. You do not have to minimize nor maximize the value of <span class="tex-span"><i>k</i></span>.</p>





```input1
0010100

```




```input2
111

```




```output1
3
3 1 3 4
3 2 5 6
1 7

```




```output2
-1

```


