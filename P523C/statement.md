## Description

<div><p>A Martian boy is named <span class="tex-span"><i>s</i></span> — he has got this name quite recently from his parents for his coming of age birthday. Now he enjoys looking for his name everywhere. If he sees that he can obtain his name from some string by removing zero or more letters (at that, the remaining letters remain in the same order), he gets happy. For example, if <span class="tex-span"><i>s</i></span>=«<span class="tex-font-style-tt">aba</span>», then strings «<span class="tex-font-style-tt">baobab</span>», «<span class="tex-font-style-tt">aabbaa</span>», «<span class="tex-font-style-tt">helloabahello</span>» make him very happy and strings «<span class="tex-font-style-tt">aab</span>», «<span class="tex-font-style-tt">baaa</span>» and «<span class="tex-font-style-tt">helloabhello</span>» do not.</p><p>However rather than being happy once, he loves twice as much being happy twice! So, when he got string <span class="tex-span"><i>t</i></span> as a present, he wanted to cut it in two parts (the left part and the right part) so that each part made him happy.</p><p>Help <span class="tex-span"><i>s</i></span> determine the number of distinct ways to cut the given string <span class="tex-span"><i>t</i></span> into two parts in the required manner.</p></div><div class="input-specification"><p>The first line contains string <span class="tex-span"><i>s</i></span>, consisting of lowercase English letters. The length of string <span class="tex-span"><i>s</i></span> is from 1 to 1000 letters.</p><p>The second line contains string <span class="tex-span"><i>t</i></span>, that also consists of lowercase English letters. The length of string <span class="tex-span"><i>t</i></span> is from 1 to <span class="tex-span">10<sup class="upper-index">6</sup></span> letters.</p></div><div class="output-specification"><p>Print the sought number of ways to cut string <span class="tex-span"><i>t</i></span> in two so that each part made <span class="tex-span"><i>s</i></span> happy. </p></div>

## Input

<p>The first line contains string <span class="tex-span"><i>s</i></span>, consisting of lowercase English letters. The length of string <span class="tex-span"><i>s</i></span> is from 1 to 1000 letters.</p><p>The second line contains string <span class="tex-span"><i>t</i></span>, that also consists of lowercase English letters. The length of string <span class="tex-span"><i>t</i></span> is from 1 to <span class="tex-span">10<sup class="upper-index">6</sup></span> letters.</p>

## Output

<p>Print the sought number of ways to cut string <span class="tex-span"><i>t</i></span> in two so that each part made <span class="tex-span"><i>s</i></span> happy. </p>





```input1
aba
baobababbah

```




```input2
mars
sunvenusearthmarsjupitersaturnuranusneptune

```




```output1
2

```




```output2
0

```


