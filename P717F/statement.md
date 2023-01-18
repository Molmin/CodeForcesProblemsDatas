## Description

<div><p>I’m strolling on sunshine, yeah-ah! And doesn’t it feel good! Well, it certainly feels good for our Heroes of Making Magic, who are casually walking on a one-directional road, fighting imps. Imps are weak and feeble creatures and they are not good at much. However, Heroes enjoy fighting them. For fun, if nothing else. </p><p>Our Hero, Ignatius, simply adores imps. He is observing a line of imps, represented as a zero-indexed array of integers <span class="tex-span"><i>a</i></span> of length <span class="tex-span"><i>n</i></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> denotes the number of imps at the <span class="tex-span"><i>i</i></span>-th position. Sometimes, imps can appear out of nowhere. When heroes fight imps, they select a segment of the line, start at one end of the segment, and finish on the other end, without ever exiting the segment. They can move exactly one cell left or right from their current position and when they do so, they defeat one imp on the cell that they moved to, so, the number of imps on that cell decreases by one. This also applies when heroes appear at one end of the segment, at the beginning of their walk. </p><p>Their goal is to defeat all imps on the segment, without ever moving to an empty cell in it (without imps), since they would get bored. Since Ignatius loves imps, he doesn’t really want to fight them, so no imps are harmed during the events of this task. However, he would like you to tell him whether it would be possible for him to clear a certain segment of imps in the above mentioned way if he wanted to. </p><p>You are given <span class="tex-span"><i>q</i></span> queries, which have two types: </p><ul>  <li> <span class="tex-span">1</span> <span class="tex-span"><i>a</i></span> <span class="tex-span"><i>b</i></span> <span class="tex-span"><i>k</i></span>&nbsp;— denotes that <span class="tex-span"><i>k</i></span> imps appear at each cell from the interval <span class="tex-span">[<i>a</i>, <i>b</i>]</span>  </li><li> <span class="tex-span">2</span> <span class="tex-span"><i>a</i></span> <span class="tex-span"><i>b</i></span> - asks whether Ignatius could defeat all imps on the interval <span class="tex-span">[<i>a</i>, <i>b</i>]</span> in the way described above </li></ul></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>), the length of the array <span class="tex-span"><i>a</i></span>. The following line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 5 000</span>), the initial number of imps in each cell. The third line contains a single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 300 000</span>), the number of queries. The remaining <span class="tex-span"><i>q</i></span> lines contain one query each. Each query is provided by integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and, possibly, <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>a</i> ≤ <i>b</i> &lt; <i>n</i></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 5 000</span>).</p></div><div class="output-specification"><p>For each second type of query output <span class="tex-span">1</span> if it is possible to clear the segment, and <span class="tex-span">0</span> if it is not.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>), the length of the array <span class="tex-span"><i>a</i></span>. The following line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 5 000</span>), the initial number of imps in each cell. The third line contains a single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 300 000</span>), the number of queries. The remaining <span class="tex-span"><i>q</i></span> lines contain one query each. Each query is provided by integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and, possibly, <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>a</i> ≤ <i>b</i> &lt; <i>n</i></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 5 000</span>).</p>

## Output

<p>For each second type of query output <span class="tex-span">1</span> if it is possible to clear the segment, and <span class="tex-span">0</span> if it is not.</p>





```input1
3
2 2 2
3
2 0 2
1 1 1 1
2 0 2

```




```output1
0
1

```



## Note

<p>For the first query, one can easily check that it is indeed impossible to get from the first to the last cell while clearing everything. After we add 1 to the second position, we can clear the segment, for example by moving in the following way: <img align="middle" class="tex-formula" src="file://31DBd739.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
