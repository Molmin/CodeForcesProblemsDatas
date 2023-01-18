## Description

<div><p>You are given two bracket sequences (not necessarily regular) $s$ and $t$ consisting only of characters '<span class="tex-font-style-tt">(</span>' and '<span class="tex-font-style-tt">)</span>'. You want to construct the shortest <span class="tex-font-style-bf">regular</span> bracket sequence that contains both given bracket sequences as <span class="tex-font-style-bf">subsequences</span> (not necessarily contiguous).</p><p>Recall what is the regular bracket sequence:</p><ul> <li> <span class="tex-font-style-tt">()</span> is the regular bracket sequence; </li><li> if $S$ is the regular bracket sequence, then <span class="tex-font-style-tt">($S$)</span> is a regular bracket sequence; </li><li> if $S$ and $T$ regular bracket sequences, then $ST$ (concatenation of $S$ and $T$) is a regular bracket sequence. </li></ul><p>Recall that the subsequence of the string $s$ is such string $t$ that can be obtained from $s$ by removing some (possibly, zero) amount of characters. For example, "<span class="tex-font-style-tt">coder</span>", "<span class="tex-font-style-tt">force</span>", "<span class="tex-font-style-tt">cf</span>" and "<span class="tex-font-style-tt">cores</span>" are subsequences of "<span class="tex-font-style-tt">codeforces</span>", but "<span class="tex-font-style-tt">fed</span>" and "<span class="tex-font-style-tt">z</span>" are not.</p></div><div class="input-specification"><p>The first line of the input contains one bracket sequence $s$ consisting of no more than $200$ characters '<span class="tex-font-style-tt">(</span>' and '<span class="tex-font-style-tt">)</span>'.</p><p>The second line of the input contains one bracket sequence $t$ consisting of no more than $200$ characters '<span class="tex-font-style-tt">(</span>' and '<span class="tex-font-style-tt">)</span>'.</p></div><div class="output-specification"><p>Print one line — the shortest <span class="tex-font-style-bf">regular</span> bracket sequence that contains both given bracket sequences as <span class="tex-font-style-bf">subsequences</span> (not necessarily contiguous). If there are several answers, you can print any.</p></div>

## Input

<p>The first line of the input contains one bracket sequence $s$ consisting of no more than $200$ characters '<span class="tex-font-style-tt">(</span>' and '<span class="tex-font-style-tt">)</span>'.</p><p>The second line of the input contains one bracket sequence $t$ consisting of no more than $200$ characters '<span class="tex-font-style-tt">(</span>' and '<span class="tex-font-style-tt">)</span>'.</p>

## Output

<p>Print one line — the shortest <span class="tex-font-style-bf">regular</span> bracket sequence that contains both given bracket sequences as <span class="tex-font-style-bf">subsequences</span> (not necessarily contiguous). If there are several answers, you can print any.</p>





```input1
(())(()
()))()
```




```input2
)
((
```




```input3
)
)))
```




```input4
())
(()(()(()(
```




```output1
(())()()
```




```output2
(())
```




```output3
((()))
```




```output4
(()()()(()()))
```


