## Description

<div><p>Ujan has a lot of numbers in his boxes. He likes order and balance, so he decided to reorder the numbers.</p><p>There are $k$ boxes numbered from $1$ to $k$. The $i$-th box contains $n_i$ integer numbers. The integers can be negative. <span class="tex-font-style-bf">All of the integers are distinct.</span> </p><p>Ujan is lazy, so he will do the following reordering of the numbers <span class="tex-font-style-bf">exactly once</span>. He will pick a single integer from each of the boxes, $k$ integers in total. Then he will insert the chosen numbers&nbsp;— one integer in each of the boxes, so that the number of integers in each box is the same as in the beginning. Note that he may also insert an integer he picked from a box back into the same box.</p><p>Ujan will be happy if the sum of the integers in each box is the same. Can he achieve this and make the boxes perfectly balanced, like all things should be?</p></div><div class="input-specification"><p>The first line contains a single integer $k$ ($1 \leq k \leq 15$), the number of boxes. </p><p>The $i$-th of the next $k$ lines first contains a single integer $n_i$ ($1 \leq n_i \leq 5\,000$), the number of integers in box $i$. Then the same line contains $n_i$ integers $a_{i,1}, \ldots, a_{i,n_i}$ ($|a_{i,j}| \leq 10^9$), the integers in the $i$-th box. </p><p>It is guaranteed that all $a_{i,j}$ are distinct.</p></div><div class="output-specification"><p>If Ujan cannot achieve his goal, output "<span class="tex-font-style-tt">No</span>" in a single line. Otherwise in the first line output "<span class="tex-font-style-tt">Yes</span>", and then output $k$ lines. The $i$-th of these lines should contain two integers $c_i$ and $p_i$. This means that Ujan should pick the integer $c_i$ from the $i$-th box and place it in the $p_i$-th box afterwards.</p><p>If there are multiple solutions, output any of those.</p><p>You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The first line contains a single integer $k$ ($1 \leq k \leq 15$), the number of boxes. </p><p>The $i$-th of the next $k$ lines first contains a single integer $n_i$ ($1 \leq n_i \leq 5\,000$), the number of integers in box $i$. Then the same line contains $n_i$ integers $a_{i,1}, \ldots, a_{i,n_i}$ ($|a_{i,j}| \leq 10^9$), the integers in the $i$-th box. </p><p>It is guaranteed that all $a_{i,j}$ are distinct.</p>

## Output

<p>If Ujan cannot achieve his goal, output "<span class="tex-font-style-tt">No</span>" in a single line. Otherwise in the first line output "<span class="tex-font-style-tt">Yes</span>", and then output $k$ lines. The $i$-th of these lines should contain two integers $c_i$ and $p_i$. This means that Ujan should pick the integer $c_i$ from the $i$-th box and place it in the $p_i$-th box afterwards.</p><p>If there are multiple solutions, output any of those.</p><p>You can print each letter in any case (upper or lower).</p>





```input1
4
3 1 7 4
2 3 2
2 8 5
1 10
```




```input2
2
2 3 -2
2 -1 5
```




```input3
2
2 -10 10
2 0 -20
```




```output1
Yes
7 2
2 3
5 1
10 4
```




```output2
No
```




```output3
Yes
-10 2
-20 1
```



## Note

<p>In the first sample, Ujan can put the number $7$ in the $2$nd box, the number $2$ in the $3$rd box, the number $5$ in the $1$st box and keep the number $10$ in the same $4$th box. Then the boxes will contain numbers $\{1,5,4\}$, $\{3, 7\}$, $\{8,2\}$ and $\{10\}$. The sum in each box then is equal to $10$.</p><p>In the second sample, it is not possible to pick and redistribute the numbers in the required way.</p><p>In the third sample, one can swap the numbers $-20$ and $-10$, making the sum in each box equal to $-10$.</p>
