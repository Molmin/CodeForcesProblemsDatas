## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem!</span></p><p>As part of your contribution in the Great Bubble War, you have been tasked with finding the newly built enemy fortress. The world you live in is a giant $10^9 \times 10^9$ grid, with squares having both coordinates between $1$ and $10^9$. </p><p>You know that the enemy base has the shape of a rectangle, with the sides parallel to the sides of the grid. The people of your world are extremely scared of being at the edge of the world, so you know that the base doesn't contain any of the squares on the edges of the grid (the $x$ or $y$ coordinate being $1$ or $10^9$). </p><p>To help you locate the base, you have been given a device that you can place in any square of the grid, and it will tell you the manhattan distance to the closest square of the base. The manhattan distance from square $(a, b)$ to square $(p, q)$ is calculated as $|a−p|+|b−q|$. If you try to place the device inside the enemy base, you will be captured by the enemy. Because of this, <span class="tex-font-style-bf">you need to make sure to never place the device inside the enemy base</span>. </p><p>Unfortunately, the device is powered by a battery and you can't recharge it. This means that you can use the device at most $40$ times. </p></div><div class="input-specification"><p>The input contains the answers to your queries. </p></div><div><h2>Interaction</h2><p>Your code is allowed to place the device on any square in the grid by writing "? $i$ $j$" $(1 \leq i,j \leq 10^9)$. In return, it will recieve the manhattan distance to the closest square of the enemy base from square $(i,j)$ or $-1$ if the square you placed the device on is inside the enemy base or outside the grid. </p><p>If you recieve $-1$ instead of a positive number, exit immidiately and you will see the <span class="tex-font-style-tt">wrong answer</span> verdict. Otherwise, you can get an arbitrary verdict because your solution will continue to read from a closed stream.</p><p>Your solution should use no more than $40$ queries. </p><p>Once you are sure where the enemy base is located, you should print "! $x$ $y$ $p$ $q$" $(1 \leq x \leq p\leq 10^9, 1 \leq y \leq q\leq 10^9)$, where $(x, y)$ is the square inside the enemy base with the smallest $x$ and $y$ coordinates, and $(p, q)$ is the square inside the enemy base with the largest $x$ and $y$ coordinates. <span class="tex-font-style-bf">Note that answering doesn't count as one of the 40 queries.</span></p><p>After printing a query or printing the answer, do not forget to output end of line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">idleness limit exceeded</span>. To do this, use: </p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> See the documentation for other languages.</li></ul></div>

## Input

<p>The input contains the answers to your queries. </p>





```input1
1
1
2
1
```




```output1
? 2 2
? 5 5
? 4 7
? 1 5
! 2 3 4 5
```


