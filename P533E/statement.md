## Description

<div><p>Analyzing the mistakes people make while typing search queries is a complex and an interesting work. As there is no guaranteed way to determine what the user originally meant by typing some query, we have to use different sorts of heuristics.</p><p>Polycarp needed to write a code that could, given two words, check whether they could have been obtained from the same word as a result of typos. Polycarpus suggested that the most common typo is skipping exactly one letter as you type a word.</p><p>Implement a program that can, given two distinct words <span class="tex-span"><i>S</i></span> and <span class="tex-span"><i>T</i></span> of the same length <span class="tex-span"><i>n</i></span> determine how many words <span class="tex-span"><i>W</i></span> of length <span class="tex-span"><i>n</i> + 1</span> are there with such property that you can transform <span class="tex-span"><i>W</i></span> into both <span class="tex-span"><i>S</i></span>, and <span class="tex-span"><i>T</i></span> by deleting exactly one character. Words <span class="tex-span"><i>S</i></span> and <span class="tex-span"><i>T</i></span> consist of lowercase English letters. Word <span class="tex-span"><i>W</i></span> also should consist of lowercase English letters.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>) — the length of words <span class="tex-span"><i>S</i></span> and <span class="tex-span"><i>T</i></span>.</p><p>The second line contains word <span class="tex-span"><i>S</i></span>.</p><p>The third line contains word <span class="tex-span"><i>T</i></span>.</p><p>Words <span class="tex-span"><i>S</i></span> and <span class="tex-span"><i>T</i></span> consist of lowercase English letters. It is guaranteed that <span class="tex-span"><i>S</i></span> and <span class="tex-span"><i>T</i></span> are distinct words.</p></div><div class="output-specification"><p>Print a single integer — the number of distinct words <span class="tex-span"><i>W</i></span> that can be transformed to <span class="tex-span"><i>S</i></span> and <span class="tex-span"><i>T</i></span> due to a typo.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>) — the length of words <span class="tex-span"><i>S</i></span> and <span class="tex-span"><i>T</i></span>.</p><p>The second line contains word <span class="tex-span"><i>S</i></span>.</p><p>The third line contains word <span class="tex-span"><i>T</i></span>.</p><p>Words <span class="tex-span"><i>S</i></span> and <span class="tex-span"><i>T</i></span> consist of lowercase English letters. It is guaranteed that <span class="tex-span"><i>S</i></span> and <span class="tex-span"><i>T</i></span> are distinct words.</p>

## Output

<p>Print a single integer — the number of distinct words <span class="tex-span"><i>W</i></span> that can be transformed to <span class="tex-span"><i>S</i></span> and <span class="tex-span"><i>T</i></span> due to a typo.</p>





```input1
7
reading
trading

```




```input2
5
sweet
sheep

```




```input3
3
toy
try

```




```output1
1

```




```output2
0

```




```output3
2

```



## Note

<p>In the first sample test the two given words could be obtained only from word "<span class="tex-font-style-tt"><span class="tex-font-style-bf">t</span>r<span class="tex-font-style-bf">e</span>ading</span>" (the deleted letters are marked in bold).</p><p>In the second sample test the two given words couldn't be obtained from the same word by removing one letter.</p><p>In the third sample test the two given words could be obtained from either word "<span class="tex-font-style-tt">t<span class="tex-font-style-bf">or</span>y</span>" or word "<span class="tex-font-style-tt">t<span class="tex-font-style-bf">ro</span>y</span>".</p>
