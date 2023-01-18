## Description

<div><p><span class="tex-font-style-it">Now that Kuroni has reached 10 years old, he is a big boy and doesn't like arrays of integers as presents anymore. This year he wants a Bracket sequence as a Birthday present. More specifically, he wants a bracket sequence so complex that no matter how hard he tries, he will not be able to remove a simple subsequence!</span></p><p>We say that a string formed by $n$ characters <span class="tex-font-style-tt">'('</span> or <span class="tex-font-style-tt">')'</span> is <span class="tex-font-style-bf">simple</span> if its length $n$ is even and positive, its first $\frac{n}{2}$ characters are <span class="tex-font-style-tt">'('</span>, and its last $\frac{n}{2}$ characters are <span class="tex-font-style-tt">')'</span>. For example, the strings <span class="tex-font-style-tt">()</span> and <span class="tex-font-style-tt">(())</span> are simple, while the strings <span class="tex-font-style-tt">)(</span> and <span class="tex-font-style-tt">()()</span> are not simple.</p><p>Kuroni will be given a string formed by characters <span class="tex-font-style-tt">'('</span> and <span class="tex-font-style-tt">')'</span> (the given string is not necessarily simple). An operation consists of choosing a subsequence of the characters of the string that forms a simple string and removing all the characters of this subsequence from the string. <span class="tex-font-style-bf">Note that this subsequence doesn't have to be continuous</span>. For example, he can apply the operation to the string <span class="tex-font-style-tt">')<span class="tex-font-style-bf">(</span>)<span class="tex-font-style-bf">(</span>()<span class="tex-font-style-bf">))</span>'</span>, to choose a subsequence of bold characters, as it forms a simple string <span class="tex-font-style-tt">'(())'</span>, delete these bold characters from the string and to get <span class="tex-font-style-tt">'))()'</span>. </p><p>Kuroni has to perform the minimum possible number of operations on the string, in such a way that no more operations can be performed on the remaining string. The resulting string <span class="tex-font-style-bf">does not</span> have to be empty.</p><p>Since the given string is too large, Kuroni is unable to figure out how to minimize the number of operations. Can you help him do it instead?</p><p>A sequence of characters $a$ is a subsequence of a string $b$ if $a$ can be obtained from $b$ by deletion of several (possibly, zero or all) characters.</p></div><div class="input-specification"><p>The only line of input contains a string $s$ ($1 \le |s| \le 1000$) formed by characters <span class="tex-font-style-tt">'('</span> and <span class="tex-font-style-tt">')'</span>, where $|s|$ is the length of $s$.</p></div><div class="output-specification"><p>In the first line, print an integer $k$ &nbsp;— the minimum number of operations you have to apply. Then, print $2k$ lines describing the operations in the following format:</p><p>For each operation, print a line containing an integer $m$ &nbsp;— the number of characters in the subsequence you will remove.</p><p>Then, print a line containing $m$ integers $1 \le a_1 &lt; a_2 &lt; \dots &lt; a_m$ &nbsp;— the indices of the characters you will remove. All integers must be less than or equal to the length of the current string, and the corresponding subsequence must form a simple string.</p><p>If there are multiple valid sequences of operations with the smallest $k$, you may print any of them.</p></div>

## Input

<p>The only line of input contains a string $s$ ($1 \le |s| \le 1000$) formed by characters <span class="tex-font-style-tt">'('</span> and <span class="tex-font-style-tt">')'</span>, where $|s|$ is the length of $s$.</p>

## Output

<p>In the first line, print an integer $k$ &nbsp;— the minimum number of operations you have to apply. Then, print $2k$ lines describing the operations in the following format:</p><p>For each operation, print a line containing an integer $m$ &nbsp;— the number of characters in the subsequence you will remove.</p><p>Then, print a line containing $m$ integers $1 \le a_1 &lt; a_2 &lt; \dots &lt; a_m$ &nbsp;— the indices of the characters you will remove. All integers must be less than or equal to the length of the current string, and the corresponding subsequence must form a simple string.</p><p>If there are multiple valid sequences of operations with the smallest $k$, you may print any of them.</p>





```input1
(()((
```




```input2
)(
```




```input3
(()())
```




```output1
1
2
1 3
```




```output2
0
```




```output3
1
4
1 2 5 6
```



## Note

<p>In the first sample, the string is '<span class="tex-font-style-tt"><span class="tex-font-style-bf">(</span>(<span class="tex-font-style-bf">)</span>((</span>'. The operation described corresponds to deleting the bolded subsequence. The resulting string is '<span class="tex-font-style-tt">(((</span>', and no more operations can be performed on it. Another valid answer is choosing indices $2$ and $3$, which results in the same final string.</p><p>In the second sample, it is already impossible to perform any operations.</p>
