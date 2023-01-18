## Description

<div><p>Professor GukiZ doesn't accept string as they are. He likes to swap some letters in string to obtain a new one.</p><p>GukiZ has strings <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, and <span class="tex-span"><i>c</i></span>. He wants to obtain string <span class="tex-span"><i>k</i></span> by swapping some letters in <span class="tex-span"><i>a</i></span>, so that <span class="tex-span"><i>k</i></span> should contain as many non-overlapping substrings equal either to <span class="tex-span"><i>b</i></span> or <span class="tex-span"><i>c</i></span> as possible. Substring of string <span class="tex-span"><i>x</i></span> is a string formed by consecutive segment of characters from <span class="tex-span"><i>x</i></span>. Two substrings of string <span class="tex-span"><i>x</i></span> overlap if there is position <span class="tex-span"><i>i</i></span> in string <span class="tex-span"><i>x</i></span> occupied by both of them.</p><p>GukiZ was disappointed because none of his students managed to solve the problem. Can you help them and find one of possible strings <span class="tex-span"><i>k</i></span>?</p></div><div class="input-specification"><p>The first line contains string <span class="tex-span"><i>a</i></span>, the second line contains string <span class="tex-span"><i>b</i></span>, and the third line contains string <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ |<i>a</i>|, |<i>b</i>|, |<i>c</i>| ≤ 10<sup class="upper-index">5</sup></span>, where <span class="tex-span">|<i>s</i>|</span> denotes the length of string <span class="tex-span"><i>s</i></span>).</p><p>All three strings consist only of lowercase English letters. </p><p>It is possible that <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> coincide.</p></div><div class="output-specification"><p>Find one of possible strings <span class="tex-span"><i>k</i></span>, as described in the problem statement. If there are multiple possible answers, print any of them.</p></div>

## Input

<p>The first line contains string <span class="tex-span"><i>a</i></span>, the second line contains string <span class="tex-span"><i>b</i></span>, and the third line contains string <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ |<i>a</i>|, |<i>b</i>|, |<i>c</i>| ≤ 10<sup class="upper-index">5</sup></span>, where <span class="tex-span">|<i>s</i>|</span> denotes the length of string <span class="tex-span"><i>s</i></span>).</p><p>All three strings consist only of lowercase English letters. </p><p>It is possible that <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> coincide.</p>

## Output

<p>Find one of possible strings <span class="tex-span"><i>k</i></span>, as described in the problem statement. If there are multiple possible answers, print any of them.</p>





```input1
aaa
a
b

```




```input2
pozdravstaklenidodiri
niste
dobri

```




```input3
abbbaaccca
ab
aca

```




```output1
aaa
```




```output2
nisteaadddiiklooprrvz
```




```output3
ababacabcc
```



## Note

<p>In the third sample, this optimal solutions has three non-overlaping substrings equal to either <span class="tex-span"><i>b</i></span> or <span class="tex-span"><i>c</i></span> on positions <span class="tex-span">1 – 2</span> (<span class="tex-span"><i>ab</i></span>), <span class="tex-span">3 – 4</span> (<span class="tex-span"><i>ab</i></span>), <span class="tex-span">5 – 7</span> (<span class="tex-span"><i>aca</i></span>). In this sample, there exist many other optimal solutions, one of them would be <span class="tex-span"><i>acaababbcc</i></span>.</p>
