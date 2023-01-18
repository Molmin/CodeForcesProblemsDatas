## Description

<div><p>Everything got unclear to us in a far away constellation Tau Ceti. Specifically, the Taucetians choose names to their children in a very peculiar manner.</p><p>Two young parents <span class="tex-font-style-tt">abac</span> and <span class="tex-font-style-tt">bbad</span> think what name to give to their first-born child. They decided that the name will be the permutation of letters of string <span class="tex-span"><i>s</i></span>. To keep up with the neighbours, they decided to call the baby so that the name was lexicographically strictly larger than the neighbour's son's name <span class="tex-span"><i>t</i></span>.</p><p>On the other hand, they suspect that a name tax will be introduced shortly. According to it, the Taucetians with lexicographically <span class="tex-font-style-it">larger</span> names will pay <span class="tex-font-style-it">larger</span> taxes. That's the reason <span class="tex-font-style-tt">abac</span> and <span class="tex-font-style-tt">bbad</span> want to call the newborn so that the name was lexicographically strictly larger than name <span class="tex-span"><i>t</i></span> and lexicographically minimum at that.</p><p>The lexicographical order of strings is the order we are all used to, the "dictionary" order. Such comparison is used in all modern programming languages to compare strings. Formally, a string <span class="tex-span"><i>p</i></span> of length <span class="tex-span"><i>n</i></span> is lexicographically less than string <span class="tex-span"><i>q</i></span> of length <span class="tex-span"><i>m</i></span>, if one of the two statements is correct:</p><ul> <li> <span class="tex-span"><i>n</i> &lt; <i>m</i></span>, and <span class="tex-span"><i>p</i></span> is the beginning (prefix) of string <span class="tex-span"><i>q</i></span> (for example, "<span class="tex-font-style-tt">aba</span>" is less than string "<span class="tex-font-style-tt">abaa</span>"), </li><li> <span class="tex-span"><i>p</i><sub class="lower-index">1</sub> = <i>q</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index">2</sub> = <i>q</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>p</i><sub class="lower-index"><i>k</i> - 1</sub> = <i>q</i><sub class="lower-index"><i>k</i> - 1</sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>k</i></sub> &lt; <i>q</i><sub class="lower-index"><i>k</i></sub></span> for some <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>min</i>(<i>n</i>, <i>m</i>)</span>), here characters in strings are numbered starting from 1. </li></ul><p>Write a program that, given string <span class="tex-span"><i>s</i></span> and the heighbours' child's name <span class="tex-span"><i>t</i></span> determines the string that is the result of permutation of letters in <span class="tex-span"><i>s</i></span>. The string should be lexicographically strictly more than <span class="tex-span"><i>t</i></span> and also, lexicographically minimum.</p></div><div class="input-specification"><p>The first line contains a non-empty string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 5000</span>), where <span class="tex-span">|<i>s</i>|</span> is its length. The second line contains a non-empty string <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ |<i>t</i>| ≤ 5000</span>), where <span class="tex-span">|<i>t</i>|</span> is its length. Both strings consist of lowercase Latin letters.</p></div><div class="output-specification"><p>Print the sought name or <span class="tex-font-style-tt">-1</span> if it doesn't exist.</p></div>

## Input

<p>The first line contains a non-empty string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 5000</span>), where <span class="tex-span">|<i>s</i>|</span> is its length. The second line contains a non-empty string <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ |<i>t</i>| ≤ 5000</span>), where <span class="tex-span">|<i>t</i>|</span> is its length. Both strings consist of lowercase Latin letters.</p>

## Output

<p>Print the sought name or <span class="tex-font-style-tt">-1</span> if it doesn't exist.</p>





```input1
aad
aac

```




```input2
abad
bob

```




```input3
abc
defg

```




```input4
czaaab
abcdef

```




```output1
aad

```




```output2
daab

```




```output3
-1

```




```output4
abczaa

```



## Note

<p>In the first sample the given string <span class="tex-span"><i>s</i></span> is the sought one, consequently, we do not need to change the letter order there.</p>
