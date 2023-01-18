## Description

<div><p><span class="tex-font-style-tt">zscoder</span> loves simple strings! A string <span class="tex-span"><i>t</i></span> is called simple if every pair of adjacent characters are distinct. For example <span class="tex-font-style-tt">ab</span>, <span class="tex-font-style-tt">aba</span>, <span class="tex-font-style-tt">zscoder</span> are simple whereas <span class="tex-font-style-tt">aa</span>, <span class="tex-font-style-tt">add</span> are not simple.</p><p><span class="tex-font-style-tt">zscoder</span> is given a string <span class="tex-span"><i>s</i></span>. He wants to change a minimum number of characters so that the string <span class="tex-span"><i>s</i></span> becomes simple. Help him with this task!</p></div><div class="input-specification"><p>The only line contains the string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 2·10<sup class="upper-index">5</sup></span>) — the string given to <span class="tex-font-style-tt">zscoder</span>. The string <span class="tex-span"><i>s</i></span> consists of only lowercase English letters.</p></div><div class="output-specification"><p>Print the simple string <span class="tex-span"><i>s</i>'</span> — the string <span class="tex-span"><i>s</i></span> after the minimal number of changes. If there are multiple solutions, you may output any of them.</p><p>Note that the string <span class="tex-span"><i>s</i>'</span> should also consist of only lowercase English letters.</p></div>

## Input

<p>The only line contains the string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 2·10<sup class="upper-index">5</sup></span>) — the string given to <span class="tex-font-style-tt">zscoder</span>. The string <span class="tex-span"><i>s</i></span> consists of only lowercase English letters.</p>

## Output

<p>Print the simple string <span class="tex-span"><i>s</i>'</span> — the string <span class="tex-span"><i>s</i></span> after the minimal number of changes. If there are multiple solutions, you may output any of them.</p><p>Note that the string <span class="tex-span"><i>s</i>'</span> should also consist of only lowercase English letters.</p>





```input1
aab

```




```input2
caaab

```




```input3
zscoder

```




```output1
bab

```




```output2
cabab

```




```output3
zscoder

```


