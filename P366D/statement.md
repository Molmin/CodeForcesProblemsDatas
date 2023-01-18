## Description

<div><p>Dima and Inna love spending time together. The problem is, Seryozha isn't too enthusiastic to leave his room for some reason. But Dima and Inna love each other so much that they decided to get criminal...</p><p>Dima constructed a trap graph. He shouted: "Hey Seryozha, have a look at my cool graph!" to get his roommate interested and kicked him into the first node.</p><p>A trap graph is an undirected graph consisting of <span class="tex-span"><i>n</i></span> nodes and <span class="tex-span"><i>m</i></span> edges. For edge number <span class="tex-span"><i>k</i></span>, Dima denoted a range of integers from <span class="tex-span"><i>l</i><sub class="lower-index"><i>k</i></sub></span> to <span class="tex-span"><i>r</i><sub class="lower-index"><i>k</i></sub></span> <span class="tex-span">(<i>l</i><sub class="lower-index"><i>k</i></sub> ≤ <i>r</i><sub class="lower-index"><i>k</i></sub>)</span>. In order to get out of the trap graph, Seryozha initially (before starting his movements) should pick some integer (let's call it <span class="tex-span"><i>x</i></span>), then Seryozha must go some way from the starting node with number <span class="tex-span">1</span> to the final node with number <span class="tex-span"><i>n</i></span>. At that, Seryozha can go along edge <span class="tex-span"><i>k</i></span> only if <span class="tex-span"><i>l</i><sub class="lower-index"><i>k</i></sub> ≤ <i>x</i> ≤ <i>r</i><sub class="lower-index"><i>k</i></sub></span>.</p><p>Seryozha is a mathematician. He defined the <span class="tex-font-style-it">loyalty</span> of some path from the <span class="tex-span">1</span>-st node to the <span class="tex-span"><i>n</i></span>-th one as the number of integers <span class="tex-span"><i>x</i></span>, such that if he initially chooses one of them, he passes the whole path. Help Seryozha find the path of maximum loyalty and return to his room as quickly as possible!</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup>, 0 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">3</sup>)</span>. Then follow <span class="tex-span"><i>m</i></span> lines describing the edges. Each line contains four integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>k</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>k</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>k</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>k</i></sub>, <i>b</i><sub class="lower-index"><i>k</i></sub> ≤ <i>n</i>, 1 ≤ <i>l</i><sub class="lower-index"><i>k</i></sub> ≤ <i>r</i><sub class="lower-index"><i>k</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span>. The numbers mean that in the trap graph the <span class="tex-span"><i>k</i></span>-th edge connects nodes <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>k</i></sub></span>, this edge corresponds to the range of integers from <span class="tex-span"><i>l</i><sub class="lower-index"><i>k</i></sub></span> to <span class="tex-span"><i>r</i><sub class="lower-index"><i>k</i></sub></span>.</p><p>Note that the given graph can have loops and multiple edges.</p></div><div class="output-specification"><p>In a single line of the output print an integer — the maximum loyalty among all paths from the first node to the <span class="tex-span"><i>n</i></span>-th one. If such paths do not exist or the maximum loyalty equals 0, print in a single line "<span class="tex-font-style-tt">Nice work, Dima!</span>" without the quotes.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup>, 0 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">3</sup>)</span>. Then follow <span class="tex-span"><i>m</i></span> lines describing the edges. Each line contains four integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>k</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>k</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>k</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>k</i></sub>, <i>b</i><sub class="lower-index"><i>k</i></sub> ≤ <i>n</i>, 1 ≤ <i>l</i><sub class="lower-index"><i>k</i></sub> ≤ <i>r</i><sub class="lower-index"><i>k</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span>. The numbers mean that in the trap graph the <span class="tex-span"><i>k</i></span>-th edge connects nodes <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>k</i></sub></span>, this edge corresponds to the range of integers from <span class="tex-span"><i>l</i><sub class="lower-index"><i>k</i></sub></span> to <span class="tex-span"><i>r</i><sub class="lower-index"><i>k</i></sub></span>.</p><p>Note that the given graph can have loops and multiple edges.</p>

## Output

<p>In a single line of the output print an integer — the maximum loyalty among all paths from the first node to the <span class="tex-span"><i>n</i></span>-th one. If such paths do not exist or the maximum loyalty equals 0, print in a single line "<span class="tex-font-style-tt">Nice work, Dima!</span>" without the quotes.</p>





```input1
4 4
1 2 1 10
2 4 3 5
1 3 1 5
2 4 2 7

```




```input2
5 6
1 2 1 10
2 5 11 20
1 4 2 5
1 3 10 11
3 4 12 10000
4 5 6 6

```




```output1
6

```




```output2
Nice work, Dima!

```



## Note

<p>Explanation of the first example.</p><p>Overall, we have 2 ways to get from node 1 to node 4: first you must go along the edge 1-2 with range [1-10], then along one of the two edges 2-4. </p><p>One of them contains range [3-5], that is, we can pass through with numbers 3, 4, 5. So the loyalty of such path is 3.</p><p>If we go along edge 2-4 with range [2-7], then we can pass through with numbers 2, 3, 4, 5, 6, 7. The loyalty is 6. That is the answer.</p><p>The edge 1-2 have no influence on the answer because its range includes both ranges of the following edges.</p>
