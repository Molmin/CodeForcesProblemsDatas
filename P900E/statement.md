## Description

<div><p>Vasya wrote down two strings <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>t</i></span> of length <span class="tex-span"><i>m</i></span> consisting of small English letters '<span class="tex-font-style-tt">a</span>' and '<span class="tex-font-style-tt">b</span>'. What is more, he knows that string <span class="tex-span"><i>t</i></span> has a form "<span class="tex-font-style-tt">abab...</span>", namely there are letters '<span class="tex-font-style-tt">a</span>' on odd positions and letters '<span class="tex-font-style-tt">b</span>' on even positions.</p><p>Suddenly in the morning, Vasya found that somebody spoiled his string. Some letters of the string <span class="tex-span"><i>s</i></span> were replaced by character '<span class="tex-font-style-tt">?</span>'.</p><p>Let's call a sequence of positions <span class="tex-span"><i>i</i>, <i>i</i> + 1, ..., <i>i</i> + <i>m</i> - 1</span> as <span class="tex-font-style-it">occurrence</span> of string <span class="tex-span"><i>t</i></span> in <span class="tex-span"><i>s</i></span>, if <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i> - <i>m</i> + 1</span> and <span class="tex-span"><i>t</i><sub class="lower-index">1</sub> = <i>s</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index">2</sub> = <i>s</i><sub class="lower-index"><i>i</i> + 1</sub>, ..., <i>t</i><sub class="lower-index"><i>m</i></sub> = <i>s</i><sub class="lower-index"><i>i</i> + <i>m</i> - 1</sub></span>.</p><p>The boy defines the <span class="tex-font-style-it">beauty</span> of the string <span class="tex-span"><i>s</i></span> as maximum number of disjoint occurrences of string <span class="tex-span"><i>t</i></span> in <span class="tex-span"><i>s</i></span>. Vasya can replace some letters '<span class="tex-font-style-tt">?</span>' with '<span class="tex-font-style-tt">a</span>' or '<span class="tex-font-style-tt">b</span>' (letters on different positions can be replaced with different letter). Vasya wants to make some replacements in such a way that beauty of string <span class="tex-span"><i>s</i></span> is maximum possible. From all such options, he wants to choose one with the minimum number of replacements. Find the number of replacements he should make.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the length of <span class="tex-span"><i>s</i></span>.</p><p>The second line contains the string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span>. It contains small English letters '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>' and characters '<span class="tex-font-style-tt">?</span>' only.</p><p>The third line contains a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the length of <span class="tex-span"><i>t</i></span>. The string <span class="tex-span"><i>t</i></span> contains letters '<span class="tex-font-style-tt">a</span>' on odd positions and '<span class="tex-font-style-tt">b</span>' on even positions.</p></div><div class="output-specification"><p>Print the only integer&nbsp;— the minimum number of replacements Vasya has to perform to make the beauty of string <span class="tex-span"><i>s</i></span> the maximum possible.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the length of <span class="tex-span"><i>s</i></span>.</p><p>The second line contains the string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span>. It contains small English letters '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>' and characters '<span class="tex-font-style-tt">?</span>' only.</p><p>The third line contains a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the length of <span class="tex-span"><i>t</i></span>. The string <span class="tex-span"><i>t</i></span> contains letters '<span class="tex-font-style-tt">a</span>' on odd positions and '<span class="tex-font-style-tt">b</span>' on even positions.</p>

## Output

<p>Print the only integer&nbsp;— the minimum number of replacements Vasya has to perform to make the beauty of string <span class="tex-span"><i>s</i></span> the maximum possible.</p>





```input1
5
bb?a?
1

```




```input2
9
ab??ab???
3

```




```output1
2

```




```output2
2

```



## Note

<p>In the first sample string <span class="tex-span"><i>t</i></span> has a form '<span class="tex-font-style-tt">a</span>'. The only optimal option is to replace all characters '<span class="tex-font-style-tt">?</span>' by '<span class="tex-font-style-tt">a</span>'.</p><p>In the second sample using two replacements we can make string equal to "<span class="tex-font-style-tt"><span class="tex-font-style-bf">aba</span>?<span class="tex-font-style-bf">aba</span>??</span>". It is impossible to get more than two occurrences.</p>
