## Description

<div><p>A string is <span class="tex-font-style-underline">binary</span>, if it consists only of characters "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">1</span>".</p><p>String <span class="tex-span"><i>v</i></span> is a <span class="tex-font-style-it">substring</span> of string <span class="tex-span"><i>w</i></span> if it has a non-zero length and can be read starting from some position in string <span class="tex-span"><i>w</i></span>. For example, string "<span class="tex-font-style-tt">010</span>" has six substrings: "<span class="tex-font-style-tt">0</span>", "<span class="tex-font-style-tt">1</span>", "<span class="tex-font-style-tt">0</span>", "<span class="tex-font-style-tt">01</span>", "<span class="tex-font-style-tt">10</span>", "<span class="tex-font-style-tt">010</span>". Two substrings are considered different if their positions of occurrence are different. So, if some string occurs multiple times, we should consider it the number of times it occurs.</p><p>You are given a binary string <span class="tex-span"><i>s</i></span>. Your task is to find the number of its substrings, containing exactly <span class="tex-span"><i>k</i></span> characters "<span class="tex-font-style-tt">1</span>".</p></div><div class="input-specification"><p>The first line contains the single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">6</sup></span>). The second line contains a non-empty binary string <span class="tex-span"><i>s</i></span>. The length of <span class="tex-span"><i>s</i></span> does not exceed <span class="tex-span">10<sup class="upper-index">6</sup></span> characters.</p></div><div class="output-specification"><p>Print the single number — the number of substrings of the given string, containing exactly <span class="tex-span"><i>k</i></span> characters "<span class="tex-font-style-tt">1</span>".</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains the single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">6</sup></span>). The second line contains a non-empty binary string <span class="tex-span"><i>s</i></span>. The length of <span class="tex-span"><i>s</i></span> does not exceed <span class="tex-span">10<sup class="upper-index">6</sup></span> characters.</p>

## Output

<p>Print the single number — the number of substrings of the given string, containing exactly <span class="tex-span"><i>k</i></span> characters "<span class="tex-font-style-tt">1</span>".</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
1
1010

```




```input2
2
01010

```




```input3
100
01010

```




```output1
6

```




```output2
4

```




```output3
0

```



## Note

<p>In the first sample the sought substrings are: "<span class="tex-font-style-tt">1</span>", "<span class="tex-font-style-tt">1</span>", "<span class="tex-font-style-tt">10</span>", "<span class="tex-font-style-tt">01</span>", "<span class="tex-font-style-tt">10</span>", "<span class="tex-font-style-tt">010</span>".</p><p>In the second sample the sought substrings are: "<span class="tex-font-style-tt">101</span>", "<span class="tex-font-style-tt">0101</span>", "<span class="tex-font-style-tt">1010</span>", "<span class="tex-font-style-tt">01010</span>".</p>
