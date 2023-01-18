## Description

<div><p>Mr. Apple, a gourmet, works as editor-in-chief of a gastronomic periodical. He travels around the world, tasting new delights of famous chefs from the most fashionable restaurants. Mr. Apple has his own signature method of review &nbsp;— in each restaurant Mr. Apple orders two sets of dishes on two different days. All the dishes are different, because Mr. Apple doesn't like to eat the same food. For each pair of dishes from different days he remembers exactly which was better, or that they were of the same quality. After this the gourmet evaluates each dish with a positive integer.</p><p>Once, during a revision of a restaurant of Celtic medieval cuisine named «Poisson», that serves chestnut soup with fir, warm soda bread, spicy lemon pie and other folk food, Mr. Apple was very pleasantly surprised the gourmet with its variety of menu, and hence ordered too much. Now he's confused about evaluating dishes.</p><p>The gourmet tasted a set of $n$ dishes on the first day and a set of $m$ dishes on the second day. He made a table $a$ of size $n \times m$, in which he described his impressions. If, according to the expert, dish $i$ from the first set was better than dish $j$ from the second set, then $a_{ij}$ is equal to "<span class="tex-font-style-tt">&gt;</span>", in the opposite case $a_{ij}$ is equal to "<span class="tex-font-style-tt">&lt;</span>". Dishes also may be equally good, in this case $a_{ij}$ is "<span class="tex-font-style-tt">=</span>".</p><p>Now Mr. Apple wants you to help him to evaluate every dish. Since Mr. Apple is very strict, he will evaluate the dishes so that the maximal number used is as small as possible. But Mr. Apple also is very fair, so he never evaluates the dishes so that it goes against his feelings. In other words, if $a_{ij}$ is "<span class="tex-font-style-tt">&lt;</span>", then the number assigned to dish $i$ from the first set should be less than the number of dish $j$ from the second set, if $a_{ij}$ is "<span class="tex-font-style-tt">&gt;</span>", then it should be greater, and finally if $a_{ij}$ is "<span class="tex-font-style-tt">=</span>", then the numbers should be the same.</p><p>Help Mr. Apple to evaluate each dish from both sets so that it is consistent with his feelings, or determine that this is impossible.</p></div><div class="input-specification"><p>The first line contains integers $n$ and $m$ ($1 \leq n, m \leq 1000$)&nbsp;— the number of dishes in both days.</p><p>Each of the next $n$ lines contains a string of $m$ symbols. The $j$-th symbol on $i$-th line is $a_{ij}$. All strings consist only of "<span class="tex-font-style-tt">&lt;</span>", "<span class="tex-font-style-tt">&gt;</span>" and "<span class="tex-font-style-tt">=</span>".</p></div><div class="output-specification"><p>The first line of output should contain "<span class="tex-font-style-tt">Yes</span>", if it's possible to do a correct evaluation for all the dishes, or "<span class="tex-font-style-tt">No</span>" otherwise.</p><p>If case an answer exist, on the second line print $n$ integers&nbsp;— evaluations of dishes from the first set, and on the third line print $m$ integers&nbsp;— evaluations of dishes from the second set.</p></div>

## Input

<p>The first line contains integers $n$ and $m$ ($1 \leq n, m \leq 1000$)&nbsp;— the number of dishes in both days.</p><p>Each of the next $n$ lines contains a string of $m$ symbols. The $j$-th symbol on $i$-th line is $a_{ij}$. All strings consist only of "<span class="tex-font-style-tt">&lt;</span>", "<span class="tex-font-style-tt">&gt;</span>" and "<span class="tex-font-style-tt">=</span>".</p>

## Output

<p>The first line of output should contain "<span class="tex-font-style-tt">Yes</span>", if it's possible to do a correct evaluation for all the dishes, or "<span class="tex-font-style-tt">No</span>" otherwise.</p><p>If case an answer exist, on the second line print $n$ integers&nbsp;— evaluations of dishes from the first set, and on the third line print $m$ integers&nbsp;— evaluations of dishes from the second set.</p>





```input1
3 4
&gt;&gt;&gt;&gt;
&gt;&gt;&gt;&gt;
&gt;&gt;&gt;&gt;
```




```input2
3 3
&gt;&gt;&gt;
&lt;&lt;&lt;
&gt;&gt;&gt;
```




```input3
3 2
==
=&lt;
==
```




```output1
Yes
2 2 2 
1 1 1 1
```




```output2
Yes
3 1 3 
2 2 2
```




```output3
No
```



## Note

<p>In the first sample, all dishes of the first day are better than dishes of the second day. So, the highest score will be $2$, for all dishes of the first day.</p><p>In the third sample, the table is contradictory&nbsp;— there is no possible evaluation of the dishes that satisfies it.</p>
