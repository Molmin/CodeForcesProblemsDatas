## Description

<div><p>Anna's got a birthday today. She invited many guests and cooked a huge (nearly infinite) birthday cake decorated by <span class="tex-span"><i>n</i></span> banana circles of different sizes. Maria's birthday is about to start in 7 minutes too, and while Anna is older, she decided to play the boss a little. She told Maria to cut the cake by <span class="tex-span"><i>k</i></span> straight-line cuts (the cutting lines can intersect) to divide banana circles into banana pieces. </p><p>Anna has many guests and she wants everyone to get at least one banana piece. That's why she told Maria to make the total number of banana pieces maximum. It's not a problem if some banana pieces end up on the same cake piece — the key is to make the maximum number of banana pieces. Determine what result Maria will achieve.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> — the number of banana circles and the number of cuts Maria should perform (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>). Next <span class="tex-span"><i>n</i></span> lines contain the positions and sizes of the banana circles (all banana circles are round). On the cake the Cartesian coordinate system is defined. Each line contains three integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>r</i></span> — the coordinates of the center of the corresponding banana piece and its radius (<span class="tex-span"> - 1000 ≤ <i>x</i>, <i>y</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>r</i> ≤ 1000</span>).</p><p>It is guaranteed that the banana circles do not intersect, do not touch each other and do not overlap with each other.</p><p>Pretest 10 is big test with <span class="tex-span"><i>n</i> = <i>k</i> = 1000</span>.</p></div><div class="output-specification"><p>Print the only integer — the largest number of banana pieces that Maria can get after she performs the <span class="tex-span"><i>k</i></span> straight-line cuts.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specificator.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> — the number of banana circles and the number of cuts Maria should perform (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>). Next <span class="tex-span"><i>n</i></span> lines contain the positions and sizes of the banana circles (all banana circles are round). On the cake the Cartesian coordinate system is defined. Each line contains three integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>r</i></span> — the coordinates of the center of the corresponding banana piece and its radius (<span class="tex-span"> - 1000 ≤ <i>x</i>, <i>y</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>r</i> ≤ 1000</span>).</p><p>It is guaranteed that the banana circles do not intersect, do not touch each other and do not overlap with each other.</p><p>Pretest 10 is big test with <span class="tex-span"><i>n</i> = <i>k</i> = 1000</span>.</p>

## Output

<p>Print the only integer — the largest number of banana pieces that Maria can get after she performs the <span class="tex-span"><i>k</i></span> straight-line cuts.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specificator.</p>





```input1
1 1
0 0 1

```




```input2
3 1
0 0 1
3 0 1
6 0 1

```




```input3
1 3
0 0 1

```




```output1
2

```




```output2
6

```




```output3
7

```


