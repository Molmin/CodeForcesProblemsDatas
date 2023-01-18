## Description

<div><p>Jabber ID on the national Berland service «Babber» has a form <span class="tex-font-style-tt">&lt;username&gt;@&lt;hostname&gt;[/resource]</span>, where </p><ul> <li> <span class="tex-font-style-tt">&lt;username&gt;</span> — is a sequence of Latin letters (lowercase or uppercase), digits or underscores characters «<span class="tex-font-style-tt">_</span>», the length of <span class="tex-font-style-tt">&lt;username&gt;</span> is between 1 and 16, inclusive. </li><li> <span class="tex-font-style-tt">&lt;hostname&gt;</span> — is a sequence of word separated by periods (characters «<span class="tex-font-style-tt">.</span>»), where each word should contain only characters allowed for <span class="tex-font-style-tt">&lt;username&gt;</span>, the length of each word is between 1 and 16, inclusive. The length of <span class="tex-font-style-tt">&lt;hostname&gt;</span> is between 1 and 32, inclusive. </li><li> <span class="tex-font-style-tt">&lt;resource&gt;</span> — is a sequence of Latin letters (lowercase or uppercase), digits or underscores characters «<span class="tex-font-style-tt">_</span>», the length of <span class="tex-font-style-tt">&lt;resource&gt;</span> is between 1 and 16, inclusive. </li></ul><p>The content of square brackets is optional — it can be present or can be absent.</p><p>There are the samples of correct Jabber IDs: <span class="tex-font-style-tt">mike@codeforces.com</span>, <span class="tex-font-style-tt">007@en.codeforces.com/contest</span>.</p><p>Your task is to write program which checks if given string is a correct Jabber ID.</p></div><div class="input-specification"><p>The input contains of a single line. The line has the length between 1 and 100 characters, inclusive. Each characters has ASCII-code between 33 and 127, inclusive.</p></div><div class="output-specification"><p>Print <span class="tex-font-style-tt">YES</span> or <span class="tex-font-style-tt">NO</span>.</p></div>

## Input

<p>The input contains of a single line. The line has the length between 1 and 100 characters, inclusive. Each characters has ASCII-code between 33 and 127, inclusive.</p>

## Output

<p>Print <span class="tex-font-style-tt">YES</span> or <span class="tex-font-style-tt">NO</span>.</p>





```input1
mike@codeforces.com

```




```input2
john.smith@codeforces.ru/contest.icpc/12

```




```output1
YES

```




```output2
NO

```


