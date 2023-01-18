## Description

<div><p>In this problem at each moment you have a set of intervals. You can move from interval <span class="tex-span">(<i>a</i>, <i>b</i>)</span> from our set to interval <span class="tex-span">(<i>c</i>, <i>d</i>)</span> from our set if and only if <span class="tex-span"><i>c</i> &lt; <i>a</i> &lt; <i>d</i></span> <span class="tex-font-style-bf">or</span> <span class="tex-span"><i>c</i> &lt; <i>b</i> &lt; <i>d</i></span>. Also there is a path from interval <span class="tex-span"><i>I</i><sub class="lower-index">1</sub></span> from our set to interval <span class="tex-span"><i>I</i><sub class="lower-index">2</sub></span> from our set if there is a sequence of successive moves starting from <span class="tex-span"><i>I</i><sub class="lower-index">1</sub></span> so that we can reach <span class="tex-span"><i>I</i><sub class="lower-index">2</sub></span>.</p><p>Your program should handle the queries of the following two types:</p><ol> <li> "<span class="tex-font-style-tt">1 x y</span>" <span class="tex-span">(<i>x</i> &lt; <i>y</i>)</span> — add the new interval <span class="tex-span">(<i>x</i>, <i>y</i>)</span> to the set of intervals. The length of the new interval is guaranteed to be strictly greater than all the previous intervals.</li><li> "<span class="tex-font-style-tt">2 a b</span>" <span class="tex-span">(<i>a</i> ≠ <i>b</i>)</span> — answer the question: is there a path from <span class="tex-span"><i>a</i></span>-th (one-based) added interval to <span class="tex-span"><i>b</i></span>-th (one-based) added interval? </li></ol><p>Answer all the queries. Note, that initially you have an empty set of intervals.</p></div><div class="input-specification"><p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> denoting the number of queries, <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. Each of the following lines contains a query as described above. All numbers in the input are integers and don't exceed <span class="tex-span">10<sup class="upper-index">9</sup></span> by their absolute value.</p><p>It's guaranteed that all queries are correct.</p></div><div class="output-specification"><p>For each query of the second type print "<span class="tex-font-style-tt">YES</span>" or "<span class="tex-font-style-tt">NO</span>" on a separate line depending on the answer.</p></div>

## Input

<p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> denoting the number of queries, <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. Each of the following lines contains a query as described above. All numbers in the input are integers and don't exceed <span class="tex-span">10<sup class="upper-index">9</sup></span> by their absolute value.</p><p>It's guaranteed that all queries are correct.</p>

## Output

<p>For each query of the second type print "<span class="tex-font-style-tt">YES</span>" or "<span class="tex-font-style-tt">NO</span>" on a separate line depending on the answer.</p>





```input1
5
1 1 5
1 5 11
2 1 2
1 2 9
2 1 2

```




```output1
NO
YES

```


