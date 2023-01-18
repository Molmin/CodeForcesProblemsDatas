## Description

<div><p>You are given a string <span class="tex-span"><i>s</i></span>, consisting of lowercase English letters, and the integer <span class="tex-span"><i>m</i></span>.</p><p>One should choose some symbols from the given string so that any contiguous subsegment of length <span class="tex-span"><i>m</i></span> has at least one selected symbol. Note that here we choose positions of symbols, not the symbols themselves.</p><p>Then one uses the chosen symbols to form <span class="tex-font-style-bf">a new string</span>. All symbols from the chosen position should be used, but we are allowed to rearrange them in any order.</p><p>Formally, we choose a subsequence of indices <span class="tex-span">1 ≤ <i>i</i><sub class="lower-index">1</sub> &lt; <i>i</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>i</i><sub class="lower-index"><i>t</i></sub> ≤ |<i>s</i>|</span>. The selected sequence must meet the following condition: for every <span class="tex-span"><i>j</i></span> such that <span class="tex-span">1 ≤ <i>j</i> ≤ |<i>s</i>| - <i>m</i> + 1</span>, there must be at least one selected index that belongs to the segment <span class="tex-span">[<i>j</i>, &nbsp;<i>j</i> + <i>m</i> - 1]</span>, i.e. there should exist a <span class="tex-span"><i>k</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>t</i></span>, such that <span class="tex-span"><i>j</i> ≤ <i>i</i><sub class="lower-index"><i>k</i></sub> ≤ <i>j</i> + <i>m</i> - 1</span>.</p><p>Then we take any permutation <span class="tex-span"><i>p</i></span> of the selected indices and form a new string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i><sub class="lower-index"><i>p</i><sub class="lower-index">1</sub></sub></sub><i>s</i><sub class="lower-index"><i>i</i><sub class="lower-index"><i>p</i><sub class="lower-index">2</sub></sub></sub>... <i>s</i><sub class="lower-index"><i>i</i><sub class="lower-index"><i>p</i><sub class="lower-index"><i>t</i></sub></sub></sub></span>.</p><p>Find the lexicographically smallest string, that can be obtained using this procedure.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 100 000</span>).</p><p>The second line contains the string <span class="tex-span"><i>s</i></span> consisting of lowercase English letters. It is guaranteed that this string is non-empty and its length doesn't exceed <span class="tex-span">100 000</span>. It is also guaranteed that the number <span class="tex-span"><i>m</i></span> doesn't exceed the length of the string <span class="tex-span"><i>s</i></span>.</p></div><div class="output-specification"><p>Print the single line containing the lexicographically smallest string, that can be obtained using the procedure described above.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 100 000</span>).</p><p>The second line contains the string <span class="tex-span"><i>s</i></span> consisting of lowercase English letters. It is guaranteed that this string is non-empty and its length doesn't exceed <span class="tex-span">100 000</span>. It is also guaranteed that the number <span class="tex-span"><i>m</i></span> doesn't exceed the length of the string <span class="tex-span"><i>s</i></span>.</p>

## Output

<p>Print the single line containing the lexicographically smallest string, that can be obtained using the procedure described above.</p>





```input1
3
cbabc

```




```input2
2
abcab

```




```input3
3
bcabcbaccba

```




```output1
a

```




```output2
aab

```




```output3
aaabb

```



## Note

<p>In the first sample, one can choose the subsequence <span class="tex-span">{3}</span> and form a string "<span class="tex-font-style-tt">a</span>".</p><p>In the second sample, one can choose the subsequence <span class="tex-span">{1, 2, 4}</span> (symbols on this positions are '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>' and '<span class="tex-font-style-tt">a</span>') and rearrange the chosen symbols to form a string "<span class="tex-font-style-tt">aab</span>".</p>
