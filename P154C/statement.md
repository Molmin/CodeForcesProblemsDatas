## Description

<div><p>You have been offered a job in a company developing a large social network. Your first task is connected with searching profiles that most probably belong to the same user.</p><p>The social network contains <span class="tex-span"><i>n</i></span> registered profiles, numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Some pairs there are friends (the "friendship" relationship is mutual, that is, if <span class="tex-span"><i>i</i></span> is friends with <span class="tex-span"><i>j</i></span>, then <span class="tex-span"><i>j</i></span> is also friends with <span class="tex-span"><i>i</i></span>). Let's say that profiles <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> (<span class="tex-span"><i>i</i> ≠ <i>j</i></span>) are <span class="tex-font-style-it">doubles</span>, if for any profile <span class="tex-span"><i>k</i></span> (<span class="tex-span"><i>k</i> ≠ <i>i</i></span>, <span class="tex-span"><i>k</i> ≠ <i>j</i></span>) one of the two statements is true: either <span class="tex-span"><i>k</i></span> is friends with <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span>, or <span class="tex-span"><i>k</i></span> isn't friends with either of them. Also, <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> can be friends or not be friends.</p><p>Your task is to count the number of different unordered pairs (<span class="tex-span"><i>i</i>, <i>j</i></span>), such that the profiles <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> are doubles. Note that the pairs are unordered, that is, pairs (<span class="tex-span"><i>a</i>, <i>b</i></span>) and (<span class="tex-span"><i>b</i>, <i>a</i></span>) are considered identical.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>), — the number of profiles and the number of pairs of friends, correspondingly. </p><p>Next <span class="tex-span"><i>m</i></span> lines contains descriptions of pairs of friends in the format "<span class="tex-span"><i>v</i> <i>u</i></span>", where <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>u</i></span> (<span class="tex-span">1 ≤ <i>v</i>, <i>u</i> ≤ <i>n</i>, <i>v</i> ≠ <i>u</i></span>) are numbers of profiles that are friends with each other. It is guaranteed that each unordered pair of friends occurs no more than once and no profile is friends with itself.</p></div><div class="output-specification"><p>Print the single integer — the number of unordered pairs of profiles that are doubles. </p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">%I64d</span> specificator.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>), — the number of profiles and the number of pairs of friends, correspondingly. </p><p>Next <span class="tex-span"><i>m</i></span> lines contains descriptions of pairs of friends in the format "<span class="tex-span"><i>v</i> <i>u</i></span>", where <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>u</i></span> (<span class="tex-span">1 ≤ <i>v</i>, <i>u</i> ≤ <i>n</i>, <i>v</i> ≠ <i>u</i></span>) are numbers of profiles that are friends with each other. It is guaranteed that each unordered pair of friends occurs no more than once and no profile is friends with itself.</p>

## Output

<p>Print the single integer — the number of unordered pairs of profiles that are doubles. </p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">%I64d</span> specificator.</p>





```input1
3 3
1 2
2 3
1 3

```




```input2
3 0

```




```input3
4 1
1 3

```




```output1
3

```




```output2
3

```




```output3
2

```



## Note

<p>In the first and second sample any two profiles are doubles.</p><p>In the third sample the doubles are pairs of profiles <span class="tex-span">(1, 3)</span> and <span class="tex-span">(2, 4)</span>.</p>
