## Description

<div><p><span class="tex-font-style-it">Yeah, we failed to make up a New Year legend for this problem</span>.</p><p>A permutation of length $n$ is an array of $n$ integers such that every integer from $1$ to $n$ appears in it exactly once. </p><p>An element $y$ of permutation $p$ is reachable from element $x$ if $x = y$, or $p_x = y$, or $p_{p_x} = y$, and so on. </p><p>The <span class="tex-font-style-bf">decomposition</span> of a permutation $p$ is defined as follows: firstly, we have a permutation $p$, all elements of which are <span class="tex-font-style-bf">not marked</span>, and an empty list $l$. Then we do the following: while there is at least one <span class="tex-font-style-bf">not marked</span> element in $p$, we find the leftmost such element, list all elements that are reachable from it <span class="tex-font-style-bf">in the order they appear in $p$</span>, mark all of these elements, then cyclically shift the list of those elements so that the maximum appears at the first position, and add this list <span class="tex-font-style-bf">as an element</span> of $l$. After all elements are marked, $l$ is the result of this decomposition.</p><p>For example, if we want to build a decomposition of $p = [5, 4, 2, 3, 1, 7, 8, 6]$, we do the following:</p><ol> <li> initially $p = [5, 4, 2, 3, 1, 7, 8, 6]$ (bold elements are marked), $l = []$; </li><li> the leftmost unmarked element is $5$; $5$ and $1$ are reachable from it, so the list we want to shift is $[5, 1]$; there is no need to shift it, since maximum is already the first element; </li><li> $p = [\textbf{5}, 4, 2, 3, \textbf{1}, 7, 8, 6]$, $l = [[5, 1]]$; </li><li> the leftmost unmarked element is $4$, the list of reachable elements is $[4, 2, 3]$; the maximum is already the first element, so there's no need to shift it; </li><li> $p = [\textbf{5}, \textbf{4}, \textbf{2}, \textbf{3}, \textbf{1}, 7, 8, 6]$, $l = [[5, 1], [4, 2, 3]]$; </li><li> the leftmost unmarked element is $7$, the list of reachable elements is $[7, 8, 6]$; we have to shift it, so it becomes $[8, 6, 7]$; </li><li> $p = [\textbf{5}, \textbf{4}, \textbf{2}, \textbf{3}, \textbf{1}, \textbf{7}, \textbf{8}, \textbf{6}]$, $l = [[5, 1], [4, 2, 3], [8, 6, 7]]$; </li><li> all elements are marked, so $[[5, 1], [4, 2, 3], [8, 6, 7]]$ is the result. </li></ol><p>The <span class="tex-font-style-it">New Year transformation</span> of a permutation is defined as follows: we build the decomposition of this permutation; then we sort all lists in decomposition in ascending order of the first elements (we don't swap the elements in these lists, only the lists themselves); then we concatenate the lists into one list which becomes a new permutation. For example, the <span class="tex-font-style-it">New Year transformation</span> of $p = [5, 4, 2, 3, 1, 7, 8, 6]$ is built as follows:</p><ol> <li> the decomposition is $[[5, 1], [4, 2, 3], [8, 6, 7]]$; </li><li> after sorting the decomposition, it becomes $[[4, 2, 3], [5, 1], [8, 6, 7]]$; </li><li> $[4, 2, 3, 5, 1, 8, 6, 7]$ is the result of the transformation. </li></ol><p>We call a permutation <span class="tex-font-style-bf">good</span> if the result of its transformation is the same as the permutation itself. For example, $[4, 3, 1, 2, 8, 5, 6, 7]$ is a good permutation; and $[5, 4, 2, 3, 1, 7, 8, 6]$ is bad, since the result of transformation is $[4, 2, 3, 5, 1, 8, 6, 7]$.</p><p>Your task is the following: given $n$ and $k$, find the $k$-th (lexicographically) good permutation of length $n$.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 1000$) — the number of test cases.</p><p>Then the test cases follow. Each test case is represented by one line containing two integers $n$ and $k$ ($1 \le n \le 50$, $1 \le k \le 10^{18}$).</p></div><div class="output-specification"><p>For each test case, print the answer to it as follows: if the number of good permutations of length $n$ is less than $k$, print one integer $-1$; otherwise, print the $k$-th good permutation on $n$ elements (in lexicographical order).</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 1000$) — the number of test cases.</p><p>Then the test cases follow. Each test case is represented by one line containing two integers $n$ and $k$ ($1 \le n \le 50$, $1 \le k \le 10^{18}$).</p>

## Output

<p>For each test case, print the answer to it as follows: if the number of good permutations of length $n$ is less than $k$, print one integer $-1$; otherwise, print the $k$-th good permutation on $n$ elements (in lexicographical order).</p>





```input1
5
3 3
5 15
4 13
6 8
4 2
```




```output1
2 1 3 
3 1 2 5 4 
-1
1 2 6 3 4 5 
1 2 4 3
```


