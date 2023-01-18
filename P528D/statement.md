## Description

<div><p>Leonid works for a small and promising start-up that works on decoding the human genome. His duties include solving complex problems of finding certain patterns in long strings consisting of letters '<span class="tex-font-style-tt">A</span>', '<span class="tex-font-style-tt">T</span>', '<span class="tex-font-style-tt">G</span>' and '<span class="tex-font-style-tt">C</span>'.</p><p>Let's consider the following scenario. There is a fragment of a human DNA chain, recorded as a string <span class="tex-span"><i>S</i></span>. To analyze the fragment, you need to find all occurrences of string <span class="tex-span"><i>T</i></span> in a string <span class="tex-span"><i>S</i></span>. However, the matter is complicated by the fact that the original chain fragment could contain minor mutations, which, however, complicate the task of finding a fragment. Leonid proposed the following approach to solve this problem.</p><p>Let's write down integer <span class="tex-span"><i>k</i> ≥ 0</span> — the error threshold. We will say that string <span class="tex-span"><i>T</i></span> occurs in string <span class="tex-span"><i>S</i></span> on position <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ |<i>S</i>| - |<i>T</i>| + 1</span>), if after putting string <span class="tex-span"><i>T</i></span> along with this position, each character of string <span class="tex-span"><i>T</i></span> corresponds to the some character of the same value in string <span class="tex-span"><i>S</i></span> at the distance of at most <span class="tex-span"><i>k</i></span>. More formally, for any <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>j</i> ≤ |<i>T</i>|</span>) there must exist such <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>p</i> ≤ |<i>S</i>|</span>), that <span class="tex-span">|(<i>i</i> + <i>j</i> - 1) - <i>p</i>| ≤ <i>k</i></span> and <span class="tex-span"><i>S</i>[<i>p</i>] = <i>T</i>[<i>j</i>]</span>.</p><p>For example, corresponding to the given definition, string "<span class="tex-font-style-tt">ACAT</span>" occurs in string "<span class="tex-font-style-tt">AGCAATTCAT</span>" in positions <span class="tex-span">2</span>, <span class="tex-span">3</span> and <span class="tex-span">6</span>.</p><center> <img class="tex-graphics" src="file://IH3UrAfN.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Note that at <span class="tex-span"><i>k</i> = 0</span> the given definition transforms to a simple definition of the occurrence of a string in a string.</p><p>Help Leonid by calculating in how many positions the given string <span class="tex-span"><i>T</i></span> occurs in the given string <span class="tex-span"><i>S</i></span> with the given error threshold.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span">|<i>S</i>|, |<i>T</i>|, <i>k</i></span> (<span class="tex-span">1 ≤ |<i>T</i>| ≤ |<i>S</i>| ≤ 200 000</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 200 000</span>) — the lengths of strings <span class="tex-span"><i>S</i></span> and <span class="tex-span"><i>T</i></span> and the error threshold.</p><p>The second line contains string <span class="tex-span"><i>S</i></span>.</p><p>The third line contains string <span class="tex-span"><i>T</i></span>.</p><p>Both strings consist only of uppercase letters '<span class="tex-font-style-tt">A</span>', '<span class="tex-font-style-tt">T</span>', '<span class="tex-font-style-tt">G</span>' and '<span class="tex-font-style-tt">C</span>'.</p></div><div class="output-specification"><p>Print a single number — the number of occurrences of <span class="tex-span"><i>T</i></span> in <span class="tex-span"><i>S</i></span> with the error threshold <span class="tex-span"><i>k</i></span> by the given definition.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span">|<i>S</i>|, |<i>T</i>|, <i>k</i></span> (<span class="tex-span">1 ≤ |<i>T</i>| ≤ |<i>S</i>| ≤ 200 000</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 200 000</span>) — the lengths of strings <span class="tex-span"><i>S</i></span> and <span class="tex-span"><i>T</i></span> and the error threshold.</p><p>The second line contains string <span class="tex-span"><i>S</i></span>.</p><p>The third line contains string <span class="tex-span"><i>T</i></span>.</p><p>Both strings consist only of uppercase letters '<span class="tex-font-style-tt">A</span>', '<span class="tex-font-style-tt">T</span>', '<span class="tex-font-style-tt">G</span>' and '<span class="tex-font-style-tt">C</span>'.</p>

## Output

<p>Print a single number — the number of occurrences of <span class="tex-span"><i>T</i></span> in <span class="tex-span"><i>S</i></span> with the error threshold <span class="tex-span"><i>k</i></span> by the given definition.</p>





```input1
10 4 1
AGCAATTCAT
ACAT

```




```output1
3

```



## Note

<p>If you happen to know about the structure of the human genome a little more than the author of the problem, and you are not impressed with Leonid's original approach, do not take everything described above seriously.</p>
