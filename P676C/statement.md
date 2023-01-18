## Description

<div><p>High school student Vasya got a string of length <span class="tex-span"><i>n</i></span> as a birthday present. This string consists of letters '<span class="tex-font-style-tt">a</span>' and '<span class="tex-font-style-tt">b</span>' only. Vasya denotes <span class="tex-font-style-it">beauty</span> of the string as the maximum length of a <span class="tex-font-style-bf">substring</span> (consecutive subsequence) consisting of equal letters.</p><p>Vasya can change no more than <span class="tex-span"><i>k</i></span> characters of the original string. What is the maximum beauty of the string he can achieve?</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000, 0 ≤ <i>k</i> ≤ <i>n</i></span>)&nbsp;— the length of the string and the maximum number of characters to change.</p><p>The second line contains the string, consisting of letters '<span class="tex-font-style-tt">a</span>' and '<span class="tex-font-style-tt">b</span>' only.</p></div><div class="output-specification"><p>Print the only integer&nbsp;— the maximum beauty of the string Vasya can achieve by changing no more than <span class="tex-span"><i>k</i></span> characters.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000, 0 ≤ <i>k</i> ≤ <i>n</i></span>)&nbsp;— the length of the string and the maximum number of characters to change.</p><p>The second line contains the string, consisting of letters '<span class="tex-font-style-tt">a</span>' and '<span class="tex-font-style-tt">b</span>' only.</p>

## Output

<p>Print the only integer&nbsp;— the maximum beauty of the string Vasya can achieve by changing no more than <span class="tex-span"><i>k</i></span> characters.</p>





```input1
4 2
abba

```




```input2
8 1
aabaabaa

```




```output1
4

```




```output2
5

```



## Note

<p>In the first sample, Vasya can obtain both strings "<span class="tex-font-style-tt">aaaa</span>" and "<span class="tex-font-style-tt">bbbb</span>".</p><p>In the second sample, the optimal answer is obtained with the string "<span class="tex-font-style-tt">aaaaabaa</span>" or with the string "<span class="tex-font-style-tt">aabaaaaa</span>".</p>
