## Description

<div><p>You are given a string <span class="tex-span"><i>S</i></span> of length <span class="tex-span"><i>n</i></span> with each character being one of the first <span class="tex-span"><i>m</i></span> lowercase English letters. </p><p>Calculate how many different strings <span class="tex-span"><i>T</i></span> of length <span class="tex-span"><i>n</i></span> composed from the first <span class="tex-span"><i>m</i></span> lowercase English letters exist such that the length of LCS (longest common subsequence) between <span class="tex-span"><i>S</i></span> and <span class="tex-span"><i>T</i></span> is <span class="tex-span"><i>n</i> - 1</span>.</p><p>Recall that LCS of two strings <span class="tex-span"><i>S</i></span> and <span class="tex-span"><i>T</i></span> is the longest string <span class="tex-span"><i>C</i></span> such that <span class="tex-span"><i>C</i></span> both in <span class="tex-span"><i>S</i></span> and <span class="tex-span"><i>T</i></span> as a subsequence.</p></div><div class="input-specification"><p>The first line contains two numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> denoting the length of string <span class="tex-span"><i>S</i></span> and number of first English lowercase characters forming the character set for strings (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">2 ≤ <i>m</i> ≤ 26</span>).</p><p>The second line contains string <span class="tex-span"><i>S</i></span>.</p></div><div class="output-specification"><p>Print the only line containing the answer.</p></div>

## Input

<p>The first line contains two numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> denoting the length of string <span class="tex-span"><i>S</i></span> and number of first English lowercase characters forming the character set for strings (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">2 ≤ <i>m</i> ≤ 26</span>).</p><p>The second line contains string <span class="tex-span"><i>S</i></span>.</p>

## Output

<p>Print the only line containing the answer.</p>





```input1
3 3
aaa

```




```input2
3 3
aab

```




```input3
1 2
a

```




```input4
10 9
abacadefgh

```




```output1
6

```




```output2
11

```




```output3
1

```




```output4
789

```



## Note

<p>For the first sample, the <span class="tex-span">6</span> possible strings <span class="tex-span"><i>T</i></span> are: <span class="tex-font-style-tt">aab</span>, <span class="tex-font-style-tt">aac</span>, <span class="tex-font-style-tt">aba</span>, <span class="tex-font-style-tt">aca</span>, <span class="tex-font-style-tt">baa</span>, <span class="tex-font-style-tt">caa</span>. </p><p>For the second sample, the <span class="tex-span">11</span> possible strings <span class="tex-span"><i>T</i></span> are: <span class="tex-font-style-tt">aaa</span>, <span class="tex-font-style-tt">aac</span>, <span class="tex-font-style-tt">aba</span>, <span class="tex-font-style-tt">abb</span>, <span class="tex-font-style-tt">abc</span>, <span class="tex-font-style-tt">aca</span>, <span class="tex-font-style-tt">acb</span>, <span class="tex-font-style-tt">baa</span>, <span class="tex-font-style-tt">bab</span>, <span class="tex-font-style-tt">caa</span>, <span class="tex-font-style-tt">cab</span>.</p><p>For the third sample, the only possible string <span class="tex-span"><i>T</i></span> is <span class="tex-font-style-tt">b</span>.</p>
