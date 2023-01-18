## Description

<div><p>You have a rectangular chocolate bar consisting of <span class="tex-span"><i>n</i> × <i>m</i></span> single squares. You want to eat <span class="tex-font-style-bf">exactly</span> <span class="tex-span"><i>k</i></span> squares, so you may need to break the chocolate bar. </p><p>In one move you can break any single rectangular piece of chocolate in two rectangular pieces. You can break only by lines between squares: horizontally or vertically. The cost of breaking is equal to square of the break length.</p><p>For example, if you have a chocolate bar consisting of <span class="tex-span">2 × 3</span> unit squares then you can break it horizontally and get two <span class="tex-span">1 × 3</span> pieces (the cost of such breaking is <span class="tex-span">3<sup class="upper-index">2</sup> = 9</span>), or you can break it vertically in two ways and get two pieces: <span class="tex-span">2 × 1</span> and <span class="tex-span">2 × 2</span> (the cost of such breaking is <span class="tex-span">2<sup class="upper-index">2</sup> = 4</span>).</p><p>For several given values <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> find the minimum total cost of breaking. You can eat exactly <span class="tex-span"><i>k</i></span> squares of chocolate if after all operations of breaking there is a set of rectangular pieces of chocolate with the total size equal to <span class="tex-span"><i>k</i></span> squares. The remaining <span class="tex-span"><i>n</i>·<i>m</i> - <i>k</i></span> squares are not necessarily form a single rectangular piece.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 40910</span>)&nbsp;— the number of values <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> to process.</p><p>Each of the next <span class="tex-span"><i>t</i></span> lines contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 30, 1 ≤ <i>k</i> ≤ <i>min</i>(<i>n</i>·<i>m</i>, 50)</span>)&nbsp;— the dimensions of the chocolate bar and the number of squares you want to eat respectively.</p></div><div class="output-specification"><p>For each <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> print the minimum total cost needed to break the chocolate bar, in order to make it possible to eat exactly <span class="tex-span"><i>k</i></span> squares.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 40910</span>)&nbsp;— the number of values <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> to process.</p><p>Each of the next <span class="tex-span"><i>t</i></span> lines contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 30, 1 ≤ <i>k</i> ≤ <i>min</i>(<i>n</i>·<i>m</i>, 50)</span>)&nbsp;— the dimensions of the chocolate bar and the number of squares you want to eat respectively.</p>

## Output

<p>For each <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> print the minimum total cost needed to break the chocolate bar, in order to make it possible to eat exactly <span class="tex-span"><i>k</i></span> squares.</p>





```input1
4
2 2 1
2 2 3
2 2 2
2 2 4

```




```output1
5
5
4
0

```



## Note

<p>In the first query of the sample one needs to perform two breaks:</p><ul> <li> to split <span class="tex-span">2 × 2</span> bar into two pieces of <span class="tex-span">2 × 1</span> (cost is <span class="tex-span">2<sup class="upper-index">2</sup> = 4</span>), </li><li> to split the resulting <span class="tex-span">2 × 1</span> into two <span class="tex-span">1 × 1</span> pieces (cost is <span class="tex-span">1<sup class="upper-index">2</sup> = 1</span>). </li></ul><p>In the second query of the sample one wants to eat <span class="tex-span">3</span> unit squares. One can use exactly the same strategy as in the first query of the sample.</p>
