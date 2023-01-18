## Description

<div><p>There are <span class="tex-span"><i>n</i></span> problems prepared for the next Codeforces round. They are arranged in ascending order by their difficulty, and no two problems have the same difficulty. Moreover, there are <span class="tex-span"><i>m</i></span> pairs of similar problems. Authors want to split problems between two division according to the following rules: </p><ul> <li> Problemset of each division should be non-empty. </li><li> Each problem should be used in exactly one division (yes, it is unusual requirement). </li><li> Each problem used in division 1 should be harder than any problem used in division 2. </li><li> If two problems are similar, they should be used in different divisions. </li></ul><p>Your goal is count the number of ways to split problem between two divisions and satisfy all the rules. Two ways to split problems are considered to be different if there is at least one problem that belongs to division 1 in one of them and to division 2 in the other.</p><p>Note, that the relation of similarity <span class="tex-font-style-bf">is not</span> transitive. That is, if problem <span class="tex-span"><i>i</i></span> is similar to problem <span class="tex-span"><i>j</i></span> and problem <span class="tex-span"><i>j</i></span> is similar to problem <span class="tex-span"><i>k</i></span>, it doesn't follow that <span class="tex-span"><i>i</i></span> is similar to <span class="tex-span"><i>k</i></span>.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 100 000</span>)&nbsp;— the number of problems prepared for the round and the number of pairs of similar problems, respectively.</p><p>Each of the following <span class="tex-span"><i>m</i></span> lines contains a pair of similar problems <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>). It's guaranteed, that no pair of problems meets twice in the input.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the number of ways to split problems in two divisions.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 100 000</span>)&nbsp;— the number of problems prepared for the round and the number of pairs of similar problems, respectively.</p><p>Each of the following <span class="tex-span"><i>m</i></span> lines contains a pair of similar problems <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>). It's guaranteed, that no pair of problems meets twice in the input.</p>

## Output

<p>Print one integer&nbsp;— the number of ways to split problems in two divisions.</p>





```input1
5 2
1 4
5 2

```




```input2
3 3
1 2
2 3
1 3

```




```input3
3 2
3 1
3 2

```




```output1
2

```




```output2
0

```




```output3
1

```



## Note

<p>In the first sample, problems <span class="tex-span">1</span> and <span class="tex-span">2</span> should be used in division 2, while problems <span class="tex-span">4</span> and <span class="tex-span">5</span> in division 1. Problem <span class="tex-span">3</span> may be used either in division 1 or in division 2.</p><p>In the second sample, all pairs of problems are similar and there is no way to split problem between two divisions without breaking any rules.</p><p>Third sample reminds you that the similarity relation is not transitive. Problem <span class="tex-span">3</span> is similar to both <span class="tex-span">1</span> and <span class="tex-span">2</span>, but <span class="tex-span">1</span> is not similar to <span class="tex-span">2</span>, so they may be used together.</p>
