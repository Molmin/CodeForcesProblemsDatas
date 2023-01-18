## Description

<div><p>Students in a class are making towers of blocks. Each student makes a (non-zero) tower by stacking pieces lengthwise on top of each other. <span class="tex-span"><i>n</i></span> of the students use pieces made of two blocks and <span class="tex-span"><i>m</i></span> of the students use pieces made of three blocks.</p><p>The students don’t want to use too many blocks, but they also want to be unique, so no two students’ towers may contain the same number of blocks. Find the minimum height necessary for the tallest of the students' towers.</p></div><div class="input-specification"><p>The first line of the input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>n</i>, <i>m</i> ≤ 1 000 000</span>, <span class="tex-span"><i>n</i> + <i>m</i> &gt; 0</span>)&nbsp;— the number of students using two-block pieces and the number of students using three-block pieces, respectively.</p></div><div class="output-specification"><p>Print a single integer, denoting the minimum possible height of the tallest tower.</p></div>

## Input

<p>The first line of the input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>n</i>, <i>m</i> ≤ 1 000 000</span>, <span class="tex-span"><i>n</i> + <i>m</i> &gt; 0</span>)&nbsp;— the number of students using two-block pieces and the number of students using three-block pieces, respectively.</p>

## Output

<p>Print a single integer, denoting the minimum possible height of the tallest tower.</p>





```input1
1 3

```




```input2
3 2

```




```input3
5 0

```




```output1
9

```




```output2
8

```




```output3
10

```



## Note

<p>In the first case, the student using two-block pieces can make a tower of height <span class="tex-span">4</span>, and the students using three-block pieces can make towers of height <span class="tex-span">3</span>, <span class="tex-span">6</span>, and <span class="tex-span">9</span> blocks. The tallest tower has a height of <span class="tex-span">9</span> blocks.</p><p>In the second case, the students can make towers of heights <span class="tex-span">2</span>, <span class="tex-span">4</span>, and <span class="tex-span">8</span> with two-block pieces and towers of heights <span class="tex-span">3</span> and <span class="tex-span">6</span> with three-block pieces, for a maximum height of <span class="tex-span">8</span> blocks.</p>
