## Description

<div><p>Today is Devu's birthday. For celebrating the occasion, he bought <span class="tex-span"><i>n</i></span> sweets from the nearby market. He has invited his <span class="tex-span"><i>f</i></span> friends. He would like to distribute the sweets among them. As he is a nice guy and the occasion is great, he doesn't want any friend to be sad, so he would ensure to give at least one sweet to each friend. </p><p>He wants to celebrate it in a unique style, so he would like to ensure following condition for the distribution of sweets. Assume that he has distributed <span class="tex-span"><i>n</i></span> sweets to his friends such that <span class="tex-span"><i>i</i><sup class="upper-index"><i>th</i></sup></span> friend is given <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> sweets. He wants to make sure that there should not be any positive integer <span class="tex-span"><i>x</i> &gt; 1</span>, which divides every <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Please find the number of ways he can distribute sweets to his friends in the required way. Note that the order of distribution is important, for example [1, 2] and [2, 1] are distinct distributions. As the answer could be very large, output answer modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p><p>To make the problem more interesting, you are given <span class="tex-span"><i>q</i></span> <span class="tex-font-style-bf">queries</span>. Each query contains an <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>f</i></span> pair. For each query please output the required number of ways modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>q</i></span> representing the number of queries <span class="tex-span">(1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup>)</span>. Each of the next <span class="tex-span"><i>q</i></span> lines contains two space space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>f</i></span> <span class="tex-span">(1 ≤ <i>f</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p></div><div class="output-specification"><p>For each query, output a single integer in a line corresponding to the answer of each query.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>q</i></span> representing the number of queries <span class="tex-span">(1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup>)</span>. Each of the next <span class="tex-span"><i>q</i></span> lines contains two space space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>f</i></span> <span class="tex-span">(1 ≤ <i>f</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p>

## Output

<p>For each query, output a single integer in a line corresponding to the answer of each query.</p>





```input1
5
6 2
7 2
6 3
6 4
7 4

```




```output1
2
6
9
10
20

```



## Note

<p>For first query: <span class="tex-span"><i>n</i> = 6, <i>f</i> = 2</span>. Possible partitions are [1, 5] and [5, 1].</p><p>For second query: <span class="tex-span"><i>n</i> = 7, <i>f</i> = 2</span>. Possible partitions are [1, 6] and [2, 5] and [3, 4] and [4, 3] and [5, 3] and [6, 1]. So in total there are 6 possible ways of partitioning.</p>
