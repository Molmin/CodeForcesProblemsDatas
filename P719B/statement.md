## Description

<div><p>Anatoly lives in the university dorm as many other students do. As you know, cockroaches are also living there together with students. Cockroaches might be of two colors: black and red. There are <span class="tex-span"><i>n</i></span> cockroaches living in Anatoly's room.</p><p>Anatoly just made all his cockroaches to form a single line. As he is a perfectionist, he would like the colors of cockroaches in the line to <span class="tex-font-style-bf">alternate</span>. He has a can of black paint and a can of red paint. In one turn he can either swap any two cockroaches, or take any single cockroach and change it's color.</p><p>Help Anatoly find out the minimum number of turns he needs to make the colors of cockroaches in the line alternate.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of cockroaches.</p><p>The second line contains a string of length <span class="tex-span"><i>n</i></span>, consisting of characters '<span class="tex-font-style-tt">b</span>' and '<span class="tex-font-style-tt">r</span>' that denote black cockroach and red cockroach respectively.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the minimum number of moves Anatoly has to perform in order to make the colors of cockroaches in the line to alternate.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of cockroaches.</p><p>The second line contains a string of length <span class="tex-span"><i>n</i></span>, consisting of characters '<span class="tex-font-style-tt">b</span>' and '<span class="tex-font-style-tt">r</span>' that denote black cockroach and red cockroach respectively.</p>

## Output

<p>Print one integer&nbsp;— the minimum number of moves Anatoly has to perform in order to make the colors of cockroaches in the line to alternate.</p>





```input1
5
rbbrr

```




```input2
5
bbbbb

```




```input3
3
rbr

```




```output1
1

```




```output2
2

```




```output3
0

```



## Note

<p>In the first sample, Anatoly has to swap third and fourth cockroaches. He needs <span class="tex-span">1</span> turn to do this.</p><p>In the second sample, the optimum answer is to paint the second and the fourth cockroaches red. This requires <span class="tex-span">2</span> turns.</p><p>In the third sample, the colors of cockroaches in the line are alternating already, thus the answer is <span class="tex-span">0</span>.</p>
