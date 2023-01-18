## Description

<div><p>Petya is a beginner programmer. He has already mastered the basics of the C++ language and moved on to learning algorithms. The first algorithm he encountered was insertion sort. Petya has already written the code that implements this algorithm and sorts the given integer zero-indexed array <span class="tex-span"><i>a</i></span> of size <span class="tex-span"><i>n</i></span> in the non-decreasing order. </p><pre class="verbatim">for (int i = 1; i &lt; n; i = i + 1)<br>{<br>   int j = i; <br>   while (j &gt; 0 &amp;&amp; a[j] &lt; a[j - 1])<br>   {<br>      swap(a[j], a[j - 1]); // swap elements a[j] and a[j - 1]<br>      j = j - 1;<br>   }<br>}<br></pre><p>Petya uses this algorithm only for sorting of arrays that are permutations of numbers from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i> - 1</span>. He has already chosen the permutation he wants to sort but he first decided to swap some two of its elements. Petya wants to choose these elements in such a way that the number of times the sorting executes function <span class="tex-font-style-tt">swap</span>, was minimum. Help Petya find out the number of ways in which he can make the swap and fulfill this requirement.</p><p>It is guaranteed that it's always possible to swap two elements of the input permutation in such a way that the number of <span class="tex-font-style-tt">swap</span> function calls decreases.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 5000</span>) — the length of the permutation. The second line contains <span class="tex-span"><i>n</i></span> different integers from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i> - 1</span>, inclusive — the actual permutation.</p></div><div class="output-specification"><p>Print two integers: the minimum number of times the <span class="tex-font-style-tt">swap</span> function is executed and the number of such pairs <span class="tex-span">(<i>i</i>, <i>j</i>)</span> that swapping the elements of the input permutation with indexes <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> leads to the minimum number of the executions.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 5000</span>) — the length of the permutation. The second line contains <span class="tex-span"><i>n</i></span> different integers from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i> - 1</span>, inclusive — the actual permutation.</p>

## Output

<p>Print two integers: the minimum number of times the <span class="tex-font-style-tt">swap</span> function is executed and the number of such pairs <span class="tex-span">(<i>i</i>, <i>j</i>)</span> that swapping the elements of the input permutation with indexes <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> leads to the minimum number of the executions.</p>





```input1
5
4 0 3 1 2

```




```input2
5
1 2 3 4 0

```




```output1
3 2

```




```output2
3 4

```



## Note

<p>In the first sample the appropriate pairs are <span class="tex-span">(0, 3)</span> and <span class="tex-span">(0, 4)</span>. </p><p>In the second sample the appropriate pairs are <span class="tex-span">(0, 4)</span>, <span class="tex-span">(1, 4)</span>, <span class="tex-span">(2, 4)</span> and <span class="tex-span">(3, 4)</span>.</p>
