## Description

<div><p>A wise man told Kerem "Different is good" once, so Kerem wants all things in his life to be different. </p><p>Kerem recently got a string <span class="tex-span"><i>s</i></span> consisting of lowercase English letters. Since Kerem likes it when things are different, he wants all <span class="tex-font-style-it">substrings</span> of his string <span class="tex-span"><i>s</i></span> to be distinct. Substring is a string formed by some number of consecutive characters of the string. For example, string "<span class="tex-font-style-tt">aba</span>" has substrings "" (empty substring), "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>", "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">ab</span>", "<span class="tex-font-style-tt">ba</span>", "<span class="tex-font-style-tt">aba</span>".</p><p>If string <span class="tex-span"><i>s</i></span> has at least two equal substrings then Kerem will change characters at some positions to some other lowercase English letters. Changing characters is a very tiring job, so Kerem want to perform as few changes as possible.</p><p>Your task is to find the minimum number of changes needed to make all the substrings of the given string distinct, or determine that it is impossible.</p></div><div class="input-specification"><p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the length of the string <span class="tex-span"><i>s</i></span>.</p><p>The second line contains the string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span> consisting of only lowercase English letters.</p></div><div class="output-specification"><p>If it's impossible to change the string <span class="tex-span"><i>s</i></span> such that all its substring are distinct print <span class="tex-font-style-tt">-1</span>. Otherwise print the minimum required number of changes.</p></div>

## Input

<p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the length of the string <span class="tex-span"><i>s</i></span>.</p><p>The second line contains the string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span> consisting of only lowercase English letters.</p>

## Output

<p>If it's impossible to change the string <span class="tex-span"><i>s</i></span> such that all its substring are distinct print <span class="tex-font-style-tt">-1</span>. Otherwise print the minimum required number of changes.</p>





```input1
2
aa

```




```input2
4
koko

```




```input3
5
murat

```




```output1
1

```




```output2
2

```




```output3
0

```



## Note

<p>In the first sample one of the possible solutions is to change the first character to '<span class="tex-font-style-tt">b</span>'.</p><p>In the second sample, one may change the first character to '<span class="tex-font-style-tt">a</span>' and second character to '<span class="tex-font-style-tt">b</span>', so the string becomes "<span class="tex-font-style-tt">abko</span>".</p>
