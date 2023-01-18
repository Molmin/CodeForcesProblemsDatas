## Description

<div><p>Suppose you have two strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>, and their length is equal. You may perform the following operation any number of times: choose two different characters <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index">2</sub></span>, and replace every occurence of <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span> in both strings with <span class="tex-span"><i>c</i><sub class="lower-index">2</sub></span>. Let's denote the <span class="tex-font-style-it">distance</span> between strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> as the minimum number of operations required to make these strings equal. For example, if <span class="tex-span"><i>s</i></span> is <span class="tex-font-style-tt">abcd</span> and <span class="tex-span"><i>t</i></span> is <span class="tex-font-style-tt">ddcb</span>, the <span class="tex-font-style-it">distance</span> between them is <span class="tex-span">2</span> — we may replace every occurence of <span class="tex-font-style-tt">a</span> with <span class="tex-font-style-tt">b</span>, so <span class="tex-span"><i>s</i></span> becomes <span class="tex-font-style-tt">bbcd</span>, and then we may replace every occurence of <span class="tex-font-style-tt">b</span> with <span class="tex-font-style-tt">d</span>, so both strings become <span class="tex-font-style-tt">ddcd</span>.</p><p>You are given two strings <span class="tex-span"><i>S</i></span> and <span class="tex-span"><i>T</i></span>. For every substring of <span class="tex-span"><i>S</i></span> consisting of <span class="tex-span">|<i>T</i>|</span> characters you have to determine the <span class="tex-font-style-it">distance</span> between this substring and <span class="tex-span"><i>T</i></span>.</p></div><div class="input-specification"><p>The first line contains the string <span class="tex-span"><i>S</i></span>, and the second — the string <span class="tex-span"><i>T</i></span> (<span class="tex-span">1 ≤ |<i>T</i>| ≤ |<i>S</i>| ≤ 125000</span>). Both strings consist of lowercase Latin letters from <span class="tex-font-style-tt">a</span> to <span class="tex-font-style-tt">f</span>.</p></div><div class="output-specification"><p>Print <span class="tex-span">|<i>S</i>| - |<i>T</i>| + 1</span> integers. The <span class="tex-span"><i>i</i></span>-th of these integers must be equal to the <span class="tex-font-style-it">distance</span> between the substring of <span class="tex-span"><i>S</i></span> beginning at <span class="tex-span"><i>i</i></span>-th index with length <span class="tex-span">|<i>T</i>|</span> and the string <span class="tex-span"><i>T</i></span>.</p></div>

## Input

<p>The first line contains the string <span class="tex-span"><i>S</i></span>, and the second — the string <span class="tex-span"><i>T</i></span> (<span class="tex-span">1 ≤ |<i>T</i>| ≤ |<i>S</i>| ≤ 125000</span>). Both strings consist of lowercase Latin letters from <span class="tex-font-style-tt">a</span> to <span class="tex-font-style-tt">f</span>.</p>

## Output

<p>Print <span class="tex-span">|<i>S</i>| - |<i>T</i>| + 1</span> integers. The <span class="tex-span"><i>i</i></span>-th of these integers must be equal to the <span class="tex-font-style-it">distance</span> between the substring of <span class="tex-span"><i>S</i></span> beginning at <span class="tex-span"><i>i</i></span>-th index with length <span class="tex-span">|<i>T</i>|</span> and the string <span class="tex-span"><i>T</i></span>.</p>





```input1
abcdefa
ddcb

```




```output1
2 3 3 3 

```


