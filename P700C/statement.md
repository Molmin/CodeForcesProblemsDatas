## Description

<div><p>Again, there are hard times in Berland! Many towns have such tensions that even civil war is possible. </p><p>There are <span class="tex-span"><i>n</i></span> towns in Reberland, some pairs of which connected by two-way roads. It is not guaranteed that it is possible to reach one town from any other town using these roads. </p><p>Towns <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> announce the final break of any relationship and intend to rule out the possibility of moving between them by the roads. Now possibly it is needed to close several roads so that moving from <span class="tex-span"><i>s</i></span> to <span class="tex-span"><i>t</i></span> using roads becomes impossible. Each town agrees to spend money on closing no more than one road, therefore, the total number of closed roads will be <span class="tex-font-style-bf">no more than two</span>.</p><p>Help them find set of no more than two roads such that there will be no way between <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> after closing these roads. For each road the budget required for its closure was estimated. Among all sets find such that the total budget for the closure of a set of roads is minimum.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 30 000</span>)&nbsp;— the number of towns in Berland and the number of roads.</p><p>The second line contains integers <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>s</i>, <i>t</i> ≤ <i>n</i></span>, <span class="tex-span"><i>s</i> ≠ <i>t</i></span>)&nbsp;— indices of towns which break up the relationships.</p><p>Then follow <span class="tex-span"><i>m</i></span> lines, each of them contains three integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— indices of towns connected by the <span class="tex-span"><i>i</i></span>-th road, and the budget on its closure.</p><p>All roads are bidirectional. It is allowed that the pair of towns is connected by more than one road. Roads that connect the city to itself are allowed. </p></div><div class="output-specification"><p>In the first line print the minimum budget required to break up the relations between <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>, if it is allowed to close no more than two roads.</p><p>In the second line print the value <span class="tex-span"><i>c</i></span> (<span class="tex-span">0 ≤ <i>c</i> ≤ 2</span>)&nbsp;— the number of roads to be closed in the found solution.</p><p>In the third line print in any order <span class="tex-span"><i>c</i></span> diverse integers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>&nbsp;— indices of closed roads. Consider that the roads are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> in the order they appear in the input. </p><p>If it is impossible to make towns <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> disconnected by removing no more than <span class="tex-span">2</span> roads, the output should contain a single line <span class="tex-font-style-tt">-1</span>. </p><p>If there are several possible answers, you may print any of them.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 30 000</span>)&nbsp;— the number of towns in Berland and the number of roads.</p><p>The second line contains integers <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>s</i>, <i>t</i> ≤ <i>n</i></span>, <span class="tex-span"><i>s</i> ≠ <i>t</i></span>)&nbsp;— indices of towns which break up the relationships.</p><p>Then follow <span class="tex-span"><i>m</i></span> lines, each of them contains three integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— indices of towns connected by the <span class="tex-span"><i>i</i></span>-th road, and the budget on its closure.</p><p>All roads are bidirectional. It is allowed that the pair of towns is connected by more than one road. Roads that connect the city to itself are allowed. </p>

## Output

<p>In the first line print the minimum budget required to break up the relations between <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>, if it is allowed to close no more than two roads.</p><p>In the second line print the value <span class="tex-span"><i>c</i></span> (<span class="tex-span">0 ≤ <i>c</i> ≤ 2</span>)&nbsp;— the number of roads to be closed in the found solution.</p><p>In the third line print in any order <span class="tex-span"><i>c</i></span> diverse integers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>&nbsp;— indices of closed roads. Consider that the roads are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> in the order they appear in the input. </p><p>If it is impossible to make towns <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> disconnected by removing no more than <span class="tex-span">2</span> roads, the output should contain a single line <span class="tex-font-style-tt">-1</span>. </p><p>If there are several possible answers, you may print any of them.</p>





```input1
6 7
1 6
2 1 6
2 3 5
3 4 9
4 6 4
4 6 5
4 5 1
3 1 3

```




```input2
6 7
1 6
2 3 1
1 2 2
1 3 3
4 5 4
3 6 5
4 6 6
1 5 7

```




```input3
5 4
1 5
2 1 3
3 2 1
3 4 4
4 5 2

```




```input4
2 3
1 2
1 2 734458840
1 2 817380027
1 2 304764803

```




```output1
8
2
2 7

```




```output2
9
2
4 5

```




```output3
1
1
2

```




```output4
-1

```


