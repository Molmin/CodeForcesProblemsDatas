## Description

<div><p>Let's suppose you have an array <span class="tex-span"><i>a</i></span>, a stack <span class="tex-span"><i>s</i></span> (initially empty) and an array <span class="tex-span"><i>b</i></span> (also initially empty).</p><p>You may perform the following operations until both <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>s</i></span> are empty:</p><ul> <li> Take the first element of <span class="tex-span"><i>a</i></span>, push it into <span class="tex-span"><i>s</i></span> and remove it from <span class="tex-span"><i>a</i></span> (if <span class="tex-span"><i>a</i></span> is not empty); </li><li> Take the top element from <span class="tex-span"><i>s</i></span>, append it to the end of array <span class="tex-span"><i>b</i></span> and remove it from <span class="tex-span"><i>s</i></span> (if <span class="tex-span"><i>s</i></span> is not empty). </li></ul><p>You can perform these operations in arbitrary order.</p><p>If there exists a way to perform the operations such that array <span class="tex-span"><i>b</i></span> is sorted in non-descending order in the end, then array <span class="tex-span"><i>a</i></span> is called <span class="tex-font-style-it">stack-sortable</span>.</p><p>For example, <span class="tex-span">[3, 1, 2]</span> is <span class="tex-font-style-it">stack-sortable</span>, because <span class="tex-span"><i>b</i></span> will be sorted if we perform the following operations:</p><ol> <li> Remove <span class="tex-span">3</span> from <span class="tex-span"><i>a</i></span> and push it into <span class="tex-span"><i>s</i></span>; </li><li> Remove <span class="tex-span">1</span> from <span class="tex-span"><i>a</i></span> and push it into <span class="tex-span"><i>s</i></span>; </li><li> Remove <span class="tex-span">1</span> from <span class="tex-span"><i>s</i></span> and append it to the end of <span class="tex-span"><i>b</i></span>; </li><li> Remove <span class="tex-span">2</span> from <span class="tex-span"><i>a</i></span> and push it into <span class="tex-span"><i>s</i></span>; </li><li> Remove <span class="tex-span">2</span> from <span class="tex-span"><i>s</i></span> and append it to the end of <span class="tex-span"><i>b</i></span>; </li><li> Remove <span class="tex-span">3</span> from <span class="tex-span"><i>s</i></span> and append it to the end of <span class="tex-span"><i>b</i></span>. </li></ol><p>After all these operations <span class="tex-span"><i>b</i> = [1, 2, 3]</span>, so <span class="tex-span">[3, 1, 2]</span> is <span class="tex-font-style-it">stack-sortable</span>. <span class="tex-span">[2, 3, 1]</span> is not <span class="tex-font-style-it">stack-sortable</span>.</p><p>You are given <span class="tex-span"><i>k</i></span> first elements of some permutation <span class="tex-span"><i>p</i></span> of size <span class="tex-span"><i>n</i></span> (recall that a permutation of size <span class="tex-span"><i>n</i></span> is an array of size <span class="tex-span"><i>n</i></span> where each integer from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> occurs exactly once). You have to restore the remaining <span class="tex-span"><i>n</i> - <i>k</i></span> elements of this permutation so it is <span class="tex-font-style-it">stack-sortable</span>. If there are multiple answers, choose the answer such that <span class="tex-span"><i>p</i></span> is lexicographically maximal (an array <span class="tex-span"><i>q</i></span> is lexicographically greater than an array <span class="tex-span"><i>p</i></span> iff there exists some integer <span class="tex-span"><i>k</i></span> such that for every <span class="tex-span"><i>i</i> &lt; <i>k</i></span> <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub> = <i>p</i><sub class="lower-index"><i>i</i></sub></span>, and <span class="tex-span"><i>q</i><sub class="lower-index"><i>k</i></sub> &gt; <i>p</i><sub class="lower-index"><i>k</i></sub></span>). <span class="tex-font-style-bf">You may not swap or change any of first <span class="tex-span"><i>k</i></span> elements of the permutation</span>.</p><p>Print the lexicographically maximal permutation <span class="tex-span"><i>p</i></span> you can obtain.</p><p>If there exists no answer then output <span class="tex-font-style-tt">-1</span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200000</span>, <span class="tex-span">1 ≤ <i>k</i> &lt; <i>n</i></span>) — the size of a desired permutation, and the number of elements you are given, respectively.</p><p>The second line contains <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>p</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the first <span class="tex-span"><i>k</i></span> elements of <span class="tex-span"><i>p</i></span>. These integers are pairwise distinct.</p></div><div class="output-specification"><p>If it is possible to restore a <span class="tex-font-style-it">stack-sortable</span> permutation <span class="tex-span"><i>p</i></span> of size <span class="tex-span"><i>n</i></span> such that the first <span class="tex-span"><i>k</i></span> elements of <span class="tex-span"><i>p</i></span> are equal to elements given in the input, print lexicographically maximal such permutation.</p><p>Otherwise print <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200000</span>, <span class="tex-span">1 ≤ <i>k</i> &lt; <i>n</i></span>) — the size of a desired permutation, and the number of elements you are given, respectively.</p><p>The second line contains <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>p</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the first <span class="tex-span"><i>k</i></span> elements of <span class="tex-span"><i>p</i></span>. These integers are pairwise distinct.</p>

## Output

<p>If it is possible to restore a <span class="tex-font-style-it">stack-sortable</span> permutation <span class="tex-span"><i>p</i></span> of size <span class="tex-span"><i>n</i></span> such that the first <span class="tex-span"><i>k</i></span> elements of <span class="tex-span"><i>p</i></span> are equal to elements given in the input, print lexicographically maximal such permutation.</p><p>Otherwise print <span class="tex-font-style-tt">-1</span>.</p>





```input1
5 3
3 2 1

```




```input2
5 3
2 3 1

```




```input3
5 1
3

```




```input4
5 2
3 4

```




```output1
3 2 1 5 4
```




```output2
-1

```




```output3
3 2 1 5 4
```




```output4
-1

```


