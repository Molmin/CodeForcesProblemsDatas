## Description

<div><p><span class="tex-font-style-bf">This is an easy version of the problem. The actual problems are different, but the easy version is almost a subtask of the hard version. Note that the constraints and the output format are different</span>.</p><p>You are given a string $s$ consisting of $n$ lowercase Latin letters.</p><p>You have to color <span class="tex-font-style-bf">all</span> its characters <span class="tex-font-style-bf">one of the two colors</span> (each character to exactly one color, the same letters can be colored the same or different colors, i.e. you can choose exactly one color for each index in $s$).</p><p>After coloring, you can swap <span class="tex-font-style-bf">any</span> two neighboring characters of the string that are colored <span class="tex-font-style-bf">different</span> colors. You can perform such an operation arbitrary (possibly, zero) number of times.</p><p>The goal is to make the string sorted, i.e. all characters should be in alphabetical order.</p><p>Your task is to say if it is possible to color the given string so that after coloring it can become sorted by <span class="tex-font-style-bf">some</span> sequence of swaps. Note that you have to restore only coloring, not the sequence of swaps.</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($1 \le n \le 200$) — the length of $s$.</p><p>The second line of the input contains the string $s$ consisting of exactly $n$ lowercase Latin letters.</p></div><div class="output-specification"><p>If it is impossible to color the given string so that after coloring it can become sorted by <span class="tex-font-style-bf">some</span> sequence of swaps, print "<span class="tex-font-style-tt">NO</span>" (without quotes) in the first line.</p><p>Otherwise, print "<span class="tex-font-style-tt">YES</span>" in the first line and <span class="tex-font-style-bf">any</span> correct coloring in the second line (the coloring is the string consisting of $n$ characters, the $i$-th character should be '<span class="tex-font-style-tt">0</span>' if the $i$-th character is colored the first color and '<span class="tex-font-style-tt">1</span>' otherwise).</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($1 \le n \le 200$) — the length of $s$.</p><p>The second line of the input contains the string $s$ consisting of exactly $n$ lowercase Latin letters.</p>

## Output

<p>If it is impossible to color the given string so that after coloring it can become sorted by <span class="tex-font-style-bf">some</span> sequence of swaps, print "<span class="tex-font-style-tt">NO</span>" (without quotes) in the first line.</p><p>Otherwise, print "<span class="tex-font-style-tt">YES</span>" in the first line and <span class="tex-font-style-bf">any</span> correct coloring in the second line (the coloring is the string consisting of $n$ characters, the $i$-th character should be '<span class="tex-font-style-tt">0</span>' if the $i$-th character is colored the first color and '<span class="tex-font-style-tt">1</span>' otherwise).</p>





```input1
9
abacbecfd
```




```input2
8
aaabbcbb
```




```input3
7
abcdedc
```




```input4
5
abcde
```




```output1
YES
001010101
```




```output2
YES
01011011
```




```output3
NO
```




```output4
YES
00000
```


