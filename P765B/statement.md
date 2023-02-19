## Description

<div><p>Kostya likes Codeforces contests very much. However, he is very disappointed that his solutions are frequently hacked. That's why he decided to obfuscate (intentionally make less readable) his code before upcoming contest.</p><p>To obfuscate the code, Kostya first looks at the first variable name used in his program and replaces all its occurrences with a single symbol <span class="tex-span"><i>a</i></span>, then he looks at the second variable name that has not been replaced yet, and replaces all its occurrences with <span class="tex-span"><i>b</i></span>, and so on. Kostya is well-mannered, so he doesn't use any one-letter names before obfuscation. Moreover, there are at most 26 unique identifiers in his programs.</p><p>You are given a list of identifiers of some program with removed spaces and line breaks. Check if this program can be a result of Kostya's obfuscation.</p></div><div class="input-specification"><p>In the only line of input there is a string <span class="tex-span"><i>S</i></span> of lowercase English letters (<span class="tex-span">1 ≤ |<i>S</i>| ≤ 500</span>)&nbsp;— the identifiers of a program with removed whitespace characters.</p></div><div class="output-specification"><p>If this program can be a result of Kostya's obfuscation, print "<span class="tex-font-style-tt">YES</span>" (without quotes), otherwise print "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>In the only line of input there is a string <span class="tex-span"><i>S</i></span> of lowercase English letters (<span class="tex-span">1 ≤ |<i>S</i>| ≤ 500</span>)&nbsp;— the identifiers of a program with removed whitespace characters.</p>

## Output

<p>If this program can be a result of Kostya's obfuscation, print "<span class="tex-font-style-tt">YES</span>" (without quotes), otherwise print "<span class="tex-font-style-tt">NO</span>".</p>





```input1
abacaba

```




```input2
jinotega

```




```output1
YES

```




```output2
NO

```



## Note

<p>In the first sample case, one possible list of identifiers would be "<span class="tex-font-style-tt">number string number character number string number</span>". Here how Kostya would obfuscate the program:</p><ul><li> replace all occurences of <span class="tex-font-style-tt">number</span> with <span class="tex-font-style-tt">a</span>, the result would be "<span class="tex-font-style-tt">a string a character a string a</span>",</li><li> replace all occurences of <span class="tex-font-style-tt">string</span> with <span class="tex-font-style-tt">b</span>, the result would be "<span class="tex-font-style-tt">a b a character a b a</span>",</li><li> replace all occurences of <span class="tex-font-style-tt">character</span> with <span class="tex-font-style-tt">c</span>, the result would be "<span class="tex-font-style-tt">a b a c a b a</span>",</li><li> all identifiers have been replaced, thus the obfuscation is finished.</li></ul>
