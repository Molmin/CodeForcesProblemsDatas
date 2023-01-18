## Description

<div><p>Calculate the minimum number of characters you need to change in the string <span class="tex-span"><i>s</i></span>, so that it contains at least <span class="tex-span"><i>k</i></span> different letters, or print that it is impossible.</p><p>String <span class="tex-span"><i>s</i></span> consists only of lowercase Latin letters, and it is allowed to change characters only to lowercase Latin letters too.</p></div><div class="input-specification"><p>First line of input contains string <span class="tex-span"><i>s</i></span>, consisting only of lowercase Latin letters (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 1000</span>, <span class="tex-span">|<i>s</i>|</span> denotes the length of <span class="tex-span"><i>s</i></span>).</p><p>Second line of input contains integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 26</span>).</p></div><div class="output-specification"><p>Print single line with a minimum number of necessary changes, or the word «<span class="tex-font-style-tt">impossible</span>» (without quotes) if it is impossible.</p></div>

## Input

<p>First line of input contains string <span class="tex-span"><i>s</i></span>, consisting only of lowercase Latin letters (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 1000</span>, <span class="tex-span">|<i>s</i>|</span> denotes the length of <span class="tex-span"><i>s</i></span>).</p><p>Second line of input contains integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 26</span>).</p>

## Output

<p>Print single line with a minimum number of necessary changes, or the word «<span class="tex-font-style-tt">impossible</span>» (without quotes) if it is impossible.</p>





```input1
yandex
6

```




```input2
yahoo
5

```




```input3
google
7

```




```output1
0

```




```output2
1

```




```output3
impossible

```



## Note

<p>In the first test case string contains <span class="tex-span">6</span> different letters, so we don't need to change anything.</p><p>In the second test case string contains <span class="tex-span">4</span> different letters: <span class="tex-span">{'<i>a</i>', '<i>h</i>', '<i>o</i>', '<i>y</i>'}</span>. To get <span class="tex-span">5</span> different letters it is necessary to change one occurrence of <span class="tex-span">'<i>o</i>'</span> to some letter, which doesn't occur in the string, for example, <span class="tex-span">{'<i>b</i>'}</span>.</p><p>In the third test case, it is impossible to make <span class="tex-span">7</span> different letters because the length of the string is <span class="tex-span">6</span>.</p>
