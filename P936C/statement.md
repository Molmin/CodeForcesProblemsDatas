## Description

<div><p>Welcome to another task about breaking the code lock! Explorers Whitfield and Martin came across an unusual safe, inside of which, according to rumors, there are untold riches, among which one can find the solution of the problem of discrete logarithm!</p><p>Of course, there is a code lock is installed on the safe. The lock has a screen that displays a string of <span class="tex-span"><i>n</i></span> lowercase Latin letters. Initially, the screen displays string <span class="tex-span"><i>s</i></span>. Whitfield and Martin found out that the safe will open when string <span class="tex-span"><i>t</i></span> will be displayed on the screen.</p><p>The string on the screen can be changed using the operation «<span class="tex-font-style-tt">shift</span> <span class="tex-span"><i>x</i></span>». In order to apply this operation, explorers choose an integer <span class="tex-span"><i>x</i></span> from 0 to <span class="tex-span"><i>n</i></span> inclusive. After that, the current string <span class="tex-span"><i>p</i> = αβ</span> changes to <span class="tex-span">β<sup class="upper-index"><i>R</i></sup>α</span>, where the length of <span class="tex-span">β</span> is <span class="tex-span"><i>x</i></span>, and the length of <span class="tex-span">α</span> is <span class="tex-span"><i>n</i> - <i>x</i></span>. In other words, the suffix of the length <span class="tex-span"><i>x</i></span> of string <span class="tex-span"><i>p</i></span> is reversed and moved to the beginning of the string. For example, after the operation «<span class="tex-font-style-tt">shift</span> <span class="tex-span">4</span>» the string «<span class="tex-font-style-tt">abcacb</span>» will be changed with string «<span class="tex-font-style-tt">bcacab</span> », since <span class="tex-span">α = </span><span class="tex-font-style-tt">ab</span>, <span class="tex-span">β = </span><span class="tex-font-style-tt">cacb</span>, <span class="tex-span">β<sup class="upper-index"><i>R</i></sup> = </span><span class="tex-font-style-tt">bcac</span>.</p><p>Explorers are afraid that if they apply too many operations «<span class="tex-font-style-tt">shift</span>», the lock will be locked forever. They ask you to find a way to get the string <span class="tex-span"><i>t</i></span> on the screen, using no more than <span class="tex-span">6100</span> operations.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span>, the length of the strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2 000</span>).</p><p>After that, there are two strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>, consisting of <span class="tex-span"><i>n</i></span> lowercase Latin letters each.</p></div><div class="output-specification"><p>If it is impossible to get string <span class="tex-span"><i>t</i></span> from string <span class="tex-span"><i>s</i></span> using no more than 6100 operations «<span class="tex-font-style-tt">shift</span>», print a single number <span class="tex-span"> - 1</span>.</p><p>Otherwise, in the first line output the number of operations <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 6100</span>). In the next line output <span class="tex-span"><i>k</i></span> numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> corresponding to the operations «<span class="tex-font-style-tt">shift</span> <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>» (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) in the order in which they should be applied.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span>, the length of the strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2 000</span>).</p><p>After that, there are two strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>, consisting of <span class="tex-span"><i>n</i></span> lowercase Latin letters each.</p>

## Output

<p>If it is impossible to get string <span class="tex-span"><i>t</i></span> from string <span class="tex-span"><i>s</i></span> using no more than 6100 operations «<span class="tex-font-style-tt">shift</span>», print a single number <span class="tex-span"> - 1</span>.</p><p>Otherwise, in the first line output the number of operations <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 6100</span>). In the next line output <span class="tex-span"><i>k</i></span> numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> corresponding to the operations «<span class="tex-font-style-tt">shift</span> <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>» (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) in the order in which they should be applied.</p>





```input1
6
abacbb
babcba

```




```input2
3
aba
bba

```




```output1
4
6 3 2 3

```




```output2
-1

```


