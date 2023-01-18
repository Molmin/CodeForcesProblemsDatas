## Description

<div><p>The Little Elephant loves playing with arrays. He has array <span class="tex-span"><i>a</i></span>, consisting of <span class="tex-span"><i>n</i></span> positive integers, indexed from 1 to <span class="tex-span"><i>n</i></span>. Let's denote the number with index <span class="tex-span"><i>i</i></span> as <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. </p><p>Additionally the Little Elephant has <span class="tex-span"><i>m</i></span> queries to the array, each query is characterised by a pair of integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>j</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>j</i></sub> ≤ <i>r</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i>)</span>. For each query <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub>, <i>r</i><sub class="lower-index"><i>j</i></sub></span> the Little Elephant has to count, how many numbers <span class="tex-span"><i>x</i></span> exist, such that number <span class="tex-span"><i>x</i></span> occurs exactly <span class="tex-span"><i>x</i></span> times among numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>l</i><sub class="lower-index"><i>j</i></sub></sub>, <i>a</i><sub class="lower-index"><i>l</i><sub class="lower-index"><i>j</i></sub> + 1</sub>, ..., <i>a</i><sub class="lower-index"><i>r</i><sub class="lower-index"><i>j</i></sub></sub></span>.</p><p>Help the Little Elephant to count the answers to all queries.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the size of array <span class="tex-span"><i>a</i></span> and the number of queries to it. The next line contains <span class="tex-span"><i>n</i></span> space-separated positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>. Next <span class="tex-span"><i>m</i></span> lines contain descriptions of queries, one per line. The <span class="tex-span"><i>j</i></span>-th of these lines contains the description of the <span class="tex-span"><i>j</i></span>-th query as two space-separated integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>j</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>j</i></sub> ≤ <i>r</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i>)</span>.</p></div><div class="output-specification"><p>In <span class="tex-span"><i>m</i></span> lines print <span class="tex-span"><i>m</i></span> integers — the answers to the queries. The <span class="tex-span"><i>j</i></span>-th line should contain the answer to the <span class="tex-span"><i>j</i></span>-th query.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the size of array <span class="tex-span"><i>a</i></span> and the number of queries to it. The next line contains <span class="tex-span"><i>n</i></span> space-separated positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>. Next <span class="tex-span"><i>m</i></span> lines contain descriptions of queries, one per line. The <span class="tex-span"><i>j</i></span>-th of these lines contains the description of the <span class="tex-span"><i>j</i></span>-th query as two space-separated integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>j</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>j</i></sub> ≤ <i>r</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i>)</span>.</p>

## Output

<p>In <span class="tex-span"><i>m</i></span> lines print <span class="tex-span"><i>m</i></span> integers — the answers to the queries. The <span class="tex-span"><i>j</i></span>-th line should contain the answer to the <span class="tex-span"><i>j</i></span>-th query.</p>





```input1
7 2
3 1 2 2 3 3 7
1 7
3 4

```




```output1
3
1

```


