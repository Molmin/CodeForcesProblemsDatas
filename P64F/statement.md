## Description

<div><p>This problem doesn't contain real-world specifications about domains, just use the problem statement as a formal document to solve the problem.</p><p>The given string <span class="tex-span"><i>s</i></span> is a domain name if it contains the characters "<span class="tex-font-style-tt">a</span>"-"<span class="tex-font-style-tt">z</span>", "<span class="tex-font-style-tt">0</span>"-"<span class="tex-font-style-tt">9</span>" and dots. No two dots shoud follow one after another (consecutive). The dots split the given string <span class="tex-span"><i>s</i></span> into the parts, the last (most right) part should have the length 2 or 3. Domain can't start or end with a dot.</p><p>You are given the string <span class="tex-span"><i>s</i></span>, check if it is domain name.</p></div><div class="input-specification"><p>The only line of the input contains given string <span class="tex-span"><i>s</i></span>. The string may contain any characters with ASCII codes from 33 to 127, inclusive. The string length is between 1 and 100, inclusive.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" if the given string <span class="tex-span"><i>s</i></span> is a domain name, or print "<span class="tex-font-style-tt">NO</span>" if it is not.</p></div>

## Input

<p>The only line of the input contains given string <span class="tex-span"><i>s</i></span>. The string may contain any characters with ASCII codes from 33 to 127, inclusive. The string length is between 1 and 100, inclusive.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" if the given string <span class="tex-span"><i>s</i></span> is a domain name, or print "<span class="tex-font-style-tt">NO</span>" if it is not.</p>





```input1
codeforces.com

```




```input2
mail.v-kontakte.ru

```




```output1
YES

```




```output2
NO

```


