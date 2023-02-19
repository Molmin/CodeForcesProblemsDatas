## Description

<div><div class="epigraph"><div class="epigraph-text"> <span class="tex-font-size-small"> For god's sake, you're boxes with legs! It is literally your only purpose! Walking onto buttons! How can you not do the one thing you were designed for?<p>Oh, that's funny, is it? Oh it's funny? Because we've been at this for twelve hours and you haven't solved it either, so I don't know why you're laughing. You've got one hour! Solve it! </p></span> </div></div><p>Wheatley decided to try to make a test chamber. He made a nice test chamber, but there was only one detail absent&nbsp;— cubes.</p><p>For completing the chamber Wheatley needs $n$ cubes. $i$-th cube has a volume $a_i$.</p><p>Wheatley has to place cubes in such a way that they would be sorted in a non-decreasing order by their volume. Formally, for each $i&gt;1$, $a_{i-1} \le a_i$ must hold.</p><p>To achieve his goal, Wheatley can exchange two <span class="tex-font-style-bf">neighbouring</span> cubes. It means that for any $i&gt;1$ you can exchange cubes on positions $i-1$ and $i$.</p><p>But there is a problem: Wheatley is very impatient. If Wheatley needs more than $\frac{n \cdot (n-1)}{2}-1$ exchange operations, he won't do this boring work.</p><p>Wheatly wants to know: can cubes be sorted under this conditions?</p></div><div class="input-specification"><p>Each test contains multiple test cases.</p><p>The first line contains one positive integer $t$ ($1 \le t \le 1000$), denoting the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains one positive integer $n$ ($2 \le n \le 5 \cdot 10^4$)&nbsp;— number of cubes.</p><p>The second line contains $n$ positive integers $a_i$ ($1 \le a_i \le 10^9$)&nbsp;— volumes of cubes.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, print a word in a single line: "<span class="tex-font-style-tt">YES</span>" (without quotation marks) if the cubes can be sorted and "<span class="tex-font-style-tt">NO</span>" (without quotation marks) otherwise.</p></div>

## Input

<p>Each test contains multiple test cases.</p><p>The first line contains one positive integer $t$ ($1 \le t \le 1000$), denoting the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains one positive integer $n$ ($2 \le n \le 5 \cdot 10^4$)&nbsp;— number of cubes.</p><p>The second line contains $n$ positive integers $a_i$ ($1 \le a_i \le 10^9$)&nbsp;— volumes of cubes.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, print a word in a single line: "<span class="tex-font-style-tt">YES</span>" (without quotation marks) if the cubes can be sorted and "<span class="tex-font-style-tt">NO</span>" (without quotation marks) otherwise.</p>





```input1
3
5
5 3 2 1 4
6
2 2 2 2 2 2
2
2 1
```




```output1
YES
YES
NO
```



## Note

<p>In the first test case it is possible to sort all the cubes in $7$ exchanges.</p><p>In the second test case the cubes are already sorted.</p><p>In the third test case we can make $0$ exchanges, but the cubes are not sorted yet, so the answer is "<span class="tex-font-style-tt">NO</span>".</p>
