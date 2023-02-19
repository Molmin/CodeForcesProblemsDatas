## Description

<div><p>You are given a string $s$ consisting of lowercase Latin letters "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>" and "<span class="tex-font-style-tt">c</span>" and question marks "<span class="tex-font-style-tt">?</span>".</p><p>Let the number of question marks in the string $s$ be $k$. Let's replace each question mark with one of the letters "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>" and "<span class="tex-font-style-tt">c</span>". Here we can obtain all $3^{k}$ possible strings consisting only of letters "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>" and "<span class="tex-font-style-tt">c</span>". For example, if $s = $"<span class="tex-font-style-tt">ac?b?c</span>" then we can obtain the following strings: $[$"<span class="tex-font-style-tt">acabac</span>", "<span class="tex-font-style-tt">acabbc</span>", "<span class="tex-font-style-tt">acabcc</span>", "<span class="tex-font-style-tt">acbbac</span>", "<span class="tex-font-style-tt">acbbbc</span>", "<span class="tex-font-style-tt">acbbcc</span>", "<span class="tex-font-style-tt">accbac</span>", "<span class="tex-font-style-tt">accbbc</span>", "<span class="tex-font-style-tt">accbcc</span>"$]$.</p><p>Your task is to count the total number of subsequences "<span class="tex-font-style-tt">abc</span>" in all resulting strings. Since the answer can be very large, print it modulo $10^{9} + 7$.</p><p>A subsequence of the string $t$ is such a sequence that can be derived from the string $t$ after removing some (possibly, zero) number of letters without changing the order of remaining letters. For example, the string "<span class="tex-font-style-tt">baacbc</span>" contains two subsequences "<span class="tex-font-style-tt">abc</span>" — a subsequence consisting of letters at positions $(2, 5, 6)$ and a subsequence consisting of letters at positions $(3, 5, 6)$.</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ $(3 \le n \le 200\,000)$ — the length of $s$.</p><p>The second line of the input contains the string $s$ of length $n$ consisting of lowercase Latin letters "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>" and "<span class="tex-font-style-tt">c</span>" and question marks"<span class="tex-font-style-tt">?</span>".</p></div><div class="output-specification"><p>Print the total number of subsequences "<span class="tex-font-style-tt">abc</span>" in all strings you can obtain if you replace all question marks with letters "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>" and "<span class="tex-font-style-tt">c</span>", modulo $10^{9} + 7$.</p></div>

## Input

<p>The first line of the input contains one integer $n$ $(3 \le n \le 200\,000)$ — the length of $s$.</p><p>The second line of the input contains the string $s$ of length $n$ consisting of lowercase Latin letters "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>" and "<span class="tex-font-style-tt">c</span>" and question marks"<span class="tex-font-style-tt">?</span>".</p>

## Output

<p>Print the total number of subsequences "<span class="tex-font-style-tt">abc</span>" in all strings you can obtain if you replace all question marks with letters "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>" and "<span class="tex-font-style-tt">c</span>", modulo $10^{9} + 7$.</p>





```input1
6
ac?b?c
```




```input2
7
???????
```




```input3
9
cccbbbaaa
```




```input4
5
a???c
```




```output1
24
```




```output2
2835
```




```output3
0
```




```output4
46
```



## Note

<p>In the first example, we can obtain $9$ strings:</p><ul> <li> "<span class="tex-font-style-tt">acabac</span>" — there are $2$ subsequences "<span class="tex-font-style-tt">abc</span>", </li><li> "<span class="tex-font-style-tt">acabbc</span>" — there are $4$ subsequences "<span class="tex-font-style-tt">abc</span>", </li><li> "<span class="tex-font-style-tt">acabcc</span>" — there are $4$ subsequences "<span class="tex-font-style-tt">abc</span>", </li><li> "<span class="tex-font-style-tt">acbbac</span>" — there are $2$ subsequences "<span class="tex-font-style-tt">abc</span>", </li><li> "<span class="tex-font-style-tt">acbbbc</span>" — there are $3$ subsequences "<span class="tex-font-style-tt">abc</span>", </li><li> "<span class="tex-font-style-tt">acbbcc</span>" — there are $4$ subsequences "<span class="tex-font-style-tt">abc</span>", </li><li> "<span class="tex-font-style-tt">accbac</span>" — there is $1$ subsequence "<span class="tex-font-style-tt">abc</span>", </li><li> "<span class="tex-font-style-tt">accbbc</span>" — there are $2$ subsequences "<span class="tex-font-style-tt">abc</span>", </li><li> "<span class="tex-font-style-tt">accbcc</span>" — there are $2$ subsequences "<span class="tex-font-style-tt">abc</span>". </li></ul><p>So, there are $2 + 4 + 4 + 2 + 3 + 4 + 1 + 2 + 2 = 24$ subsequences "<span class="tex-font-style-tt">abc</span>" in total.</p>
