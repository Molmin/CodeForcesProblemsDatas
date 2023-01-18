## Description

<div><p>There are two strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>, consisting only of letters <span class="tex-font-style-tt">a</span> and <span class="tex-font-style-tt">b</span>. You can make the following operation several times: choose a prefix of <span class="tex-span"><i>s</i></span>, a prefix of <span class="tex-span"><i>t</i></span> and swap them. Prefixes <span class="tex-font-style-underline">can be empty</span>, also a prefix can coincide with a whole string. </p><p>Your task is to find a sequence of operations after which one of the strings consists only of <span class="tex-font-style-tt">a</span> letters and the other consists only of <span class="tex-font-style-tt">b</span> letters. The number of operations should be <span class="tex-font-style-underline">minimized</span>.</p></div><div class="input-specification"><p>The first line contains a string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 2·10<sup class="upper-index">5</sup></span>).</p><p>The second line contains a string <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ |<i>t</i>| ≤ 2·10<sup class="upper-index">5</sup></span>).</p><p>Here <span class="tex-span">|<i>s</i>|</span> and <span class="tex-span">|<i>t</i>|</span> denote the lengths of <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>, respectively. It is guaranteed that at least one of the strings contains at least one <span class="tex-font-style-tt">a</span> letter and at least one of the strings contains at least one <span class="tex-font-style-tt">b</span> letter.</p></div><div class="output-specification"><p>The first line should contain a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of operations.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines should contain two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— the lengths of prefixes of <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> to swap, respectively.</p><p>If there are multiple possible solutions, you can print any of them. It's guaranteed that a solution with given constraints exists.</p></div>

## Input

<p>The first line contains a string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 2·10<sup class="upper-index">5</sup></span>).</p><p>The second line contains a string <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ |<i>t</i>| ≤ 2·10<sup class="upper-index">5</sup></span>).</p><p>Here <span class="tex-span">|<i>s</i>|</span> and <span class="tex-span">|<i>t</i>|</span> denote the lengths of <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>, respectively. It is guaranteed that at least one of the strings contains at least one <span class="tex-font-style-tt">a</span> letter and at least one of the strings contains at least one <span class="tex-font-style-tt">b</span> letter.</p>

## Output

<p>The first line should contain a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of operations.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines should contain two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— the lengths of prefixes of <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> to swap, respectively.</p><p>If there are multiple possible solutions, you can print any of them. It's guaranteed that a solution with given constraints exists.</p>





```input1
bab
bb

```




```input2
bbbb
aaa

```




```output1
2
1 0
1 3

```




```output2
0

```



## Note

<p>In the first example, you can solve the problem in two operations:</p><ol> <li> Swap the prefix of the first string with length <span class="tex-span">1</span> and the prefix of the second string with length <span class="tex-span">0</span>. After this swap, you'll have strings <span class="tex-font-style-tt">ab</span> and <span class="tex-font-style-tt">bbb</span>. </li><li> Swap the prefix of the first string with length <span class="tex-span">1</span> and the prefix of the second string with length <span class="tex-span">3</span>. After this swap, you'll have strings <span class="tex-font-style-tt">bbbb</span> and <span class="tex-font-style-tt">a</span>. </li></ol><p>In the second example, the strings are already appropriate, so no operations are needed.</p>
