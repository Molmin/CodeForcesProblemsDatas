## Description

<div><p>Our bear's forest has a checkered field. The checkered field is an <span class="tex-span"><i>n</i> × <i>n</i></span> table, the rows are numbered from 1 to <span class="tex-span"><i>n</i></span> from top to bottom, the columns are numbered from 1 to <span class="tex-span"><i>n</i></span> from left to right. Let's denote a cell of the field on the intersection of row <span class="tex-span"><i>x</i></span> and column <span class="tex-span"><i>y</i></span> by record <span class="tex-span">(<i>x</i>, <i>y</i>)</span>. Each cell of the field contains growing raspberry, at that, the cell <span class="tex-span">(<i>x</i>, <i>y</i>)</span> of the field contains <span class="tex-span"><i>x</i> + <i>y</i></span> raspberry bushes.</p><p>The bear came out to walk across the field. At the beginning of the walk his speed is <span class="tex-span">(<i>dx</i>, <i>dy</i>)</span>. Then the bear spends exactly <span class="tex-span"><i>t</i></span> seconds on the field. Each second the following takes place:</p><ul> <li> Let's suppose that at the current moment the bear is in cell <span class="tex-span">(<i>x</i>, <i>y</i>)</span>. </li><li> First the bear eats the raspberry from all the bushes he has in the current cell. After the bear eats the raspberry from <span class="tex-span"><i>k</i></span> bushes, he increases each component of his speed by <span class="tex-span"><i>k</i></span>. In other words, if before eating the <span class="tex-span"><i>k</i></span> bushes of raspberry his speed was <span class="tex-span">(<i>dx</i>, <i>dy</i>)</span>, then after eating the berry his speed equals <span class="tex-span">(<i>dx</i> + <i>k</i>, <i>dy</i> + <i>k</i>)</span>. </li><li> Let's denote the current speed of the bear <span class="tex-span">(<i>dx</i>, <i>dy</i>)</span> (it was increased after the previous step). Then the bear moves from cell <span class="tex-span">(<i>x</i>, <i>y</i>)</span> to cell <span class="tex-span">(((<i>x</i> + <i>dx</i> - 1)&nbsp;<i>mod</i>&nbsp;<i>n</i>) + 1, ((<i>y</i> + <i>dy</i> - 1)&nbsp;<i>mod</i>&nbsp;<i>n</i>) + 1)</span>. </li><li> Then one additional raspberry bush grows in each cell of the field. </li></ul><p>You task is to predict the bear's actions. Find the cell he ends up in if he starts from cell <span class="tex-span">(<i>sx</i>, <i>sy</i>)</span>. Assume that each bush has infinitely much raspberry and the bear will never eat all of it.</p></div><div class="input-specification"><p>The first line of the input contains six space-separated integers: <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>sx</i></span>, <span class="tex-span"><i>sy</i></span>, <span class="tex-span"><i>dx</i></span>, <span class="tex-span"><i>dy</i></span>, <span class="tex-span"><i>t</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup>;&nbsp;1 ≤ <i>sx</i>, <i>sy</i> ≤ <i>n</i>;&nbsp; - 100 ≤ <i>dx</i>, <i>dy</i> ≤ 100;&nbsp;0 ≤ <i>t</i> ≤ 10<sup class="upper-index">18</sup>)</span>.</p></div><div class="output-specification"><p>Print two integers — the coordinates of the cell the bear will end up in after <span class="tex-span"><i>t</i></span> seconds.</p></div>

## Input

<p>The first line of the input contains six space-separated integers: <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>sx</i></span>, <span class="tex-span"><i>sy</i></span>, <span class="tex-span"><i>dx</i></span>, <span class="tex-span"><i>dy</i></span>, <span class="tex-span"><i>t</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup>;&nbsp;1 ≤ <i>sx</i>, <i>sy</i> ≤ <i>n</i>;&nbsp; - 100 ≤ <i>dx</i>, <i>dy</i> ≤ 100;&nbsp;0 ≤ <i>t</i> ≤ 10<sup class="upper-index">18</sup>)</span>.</p>

## Output

<p>Print two integers — the coordinates of the cell the bear will end up in after <span class="tex-span"><i>t</i></span> seconds.</p>





```input1
5 1 2 0 1 2

```




```input2
1 1 1 -1 -1 2

```




```output1
3 1
```




```output2
1 1
```



## Note

<p>Operation <span class="tex-span"><i>a</i>&nbsp;<i>mod</i>&nbsp;<i>b</i></span> means taking the remainder after dividing <span class="tex-span"><i>a</i></span> by <span class="tex-span"><i>b</i></span>. Note that the result of the operation is always non-negative. For example, <span class="tex-span">( - 1)&nbsp;<i>mod</i>&nbsp;3 = 2</span>.</p><p>In the first sample before the first move the speed vector will equal (3,4) and the bear will get to cell (4,1). Before the second move the speed vector will equal (9,10) and he bear will get to cell (3,1). Don't forget that at the second move, the number of berry bushes increased by 1.</p><p>In the second sample before the first move the speed vector will equal (1,1) and the bear will get to cell (1,1). Before the second move, the speed vector will equal (4,4) and the bear will get to cell (1,1). Don't forget that at the second move, the number of berry bushes increased by 1.</p>
