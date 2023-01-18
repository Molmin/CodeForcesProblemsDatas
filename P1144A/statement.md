## Description

<div><p>A string is called <span class="tex-font-style-it">diverse</span> if it contains consecutive (adjacent) letters of the Latin alphabet and each letter occurs exactly once. For example, the following strings are diverse: "<span class="tex-font-style-tt">fced</span>", "<span class="tex-font-style-tt">xyz</span>", "<span class="tex-font-style-tt">r</span>" and "<span class="tex-font-style-tt">dabcef</span>". The following string are <span class="tex-font-style-bf">not</span> diverse: "<span class="tex-font-style-tt">az</span>", "<span class="tex-font-style-tt">aa</span>", "<span class="tex-font-style-tt">bad</span>" and "<span class="tex-font-style-tt">babc</span>". Note that the letters '<span class="tex-font-style-tt">a</span>' and '<span class="tex-font-style-tt">z</span>' are not adjacent.</p><p>Formally, consider positions of all letters in the string in the alphabet. These positions should form contiguous segment, i.e. they should come one by one without any gaps. And all letters in the string should be distinct (duplicates are not allowed).</p><p>You are given a sequence of strings. For each string, if it is diverse, print "<span class="tex-font-style-tt">Yes</span>". Otherwise, print "<span class="tex-font-style-tt">No</span>".</p></div><div class="input-specification"><p>The first line contains integer $n$ ($1 \le n \le 100$), denoting the number of strings to process. The following $n$ lines contains strings, one string per line. Each string contains only lowercase Latin letters, its length is between $1$ and $100$, inclusive.</p></div><div class="output-specification"><p>Print $n$ lines, one line per a string in the input. The line should contain "<span class="tex-font-style-tt">Yes</span>" if the corresponding string is diverse and "<span class="tex-font-style-tt">No</span>" if the corresponding string is not diverse. You can print each letter in any case (upper or lower). For example, "<span class="tex-font-style-tt">YeS</span>", "<span class="tex-font-style-tt">no</span>" and "<span class="tex-font-style-tt">yES</span>" are all acceptable.</p></div>

## Input

<p>The first line contains integer $n$ ($1 \le n \le 100$), denoting the number of strings to process. The following $n$ lines contains strings, one string per line. Each string contains only lowercase Latin letters, its length is between $1$ and $100$, inclusive.</p>

## Output

<p>Print $n$ lines, one line per a string in the input. The line should contain "<span class="tex-font-style-tt">Yes</span>" if the corresponding string is diverse and "<span class="tex-font-style-tt">No</span>" if the corresponding string is not diverse. You can print each letter in any case (upper or lower). For example, "<span class="tex-font-style-tt">YeS</span>", "<span class="tex-font-style-tt">no</span>" and "<span class="tex-font-style-tt">yES</span>" are all acceptable.</p>





```input1
8
fced
xyz
r
dabcef
az
aa
bad
babc
```




```output1
Yes
Yes
Yes
Yes
No
No
No
No
```


