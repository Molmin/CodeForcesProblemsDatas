## Description

<div><p>Annie has gotten bored of winning every coding contest and farming unlimited rating. Today, she is going to farm potatoes instead.</p><p>Annie's garden is an infinite 2D plane. She has $n$ potatoes to plant, and the $i$-th potato must be planted at $(x_i,y_i)$. Starting at the point $(0, 0)$, Annie begins walking, in one step she can travel one unit <span class="tex-font-style-bf">right</span> or <span class="tex-font-style-bf">up</span> (increasing her $x$ or $y$ coordinate by $1$ respectively). At any point $(X,Y)$ during her walk she can plant some potatoes at arbitrary points using her potato gun, consuming $\max(|X-x|,|Y-y|)$ units of energy in order to plant a potato at $(x,y)$. Find the minimum total energy required to plant every potato.</p><p>Note that Annie may plant any number of potatoes from any point.</p></div><div class="input-specification"><p>The first line contains the integer $n$ ($1 \le n \le 800\,000$).</p><p>The next $n$ lines contain two integers $x_i$ and $y_i$ ($0 \le x_i,y_i \le 10^9$), representing the location of the $i$-th potato. It is possible that some potatoes should be planted in the same location.</p></div><div class="output-specification"><p>Print the minimum total energy to plant all potatoes.</p></div>

## Input

<p>The first line contains the integer $n$ ($1 \le n \le 800\,000$).</p><p>The next $n$ lines contain two integers $x_i$ and $y_i$ ($0 \le x_i,y_i \le 10^9$), representing the location of the $i$-th potato. It is possible that some potatoes should be planted in the same location.</p>

## Output

<p>Print the minimum total energy to plant all potatoes.</p>





```input1
2
1 1
2 2
```




```input2
2
1 1
2 0
```




```input3
3
5 5
7 7
4 9
```




```input4
10
5 1
4 0
9 6
0 2
10 1
9 10
3 10
0 10
8 9
1 5
```




```input5
10
1 1
2 2
2 0
4 2
4 0
2 0
0 2
4 0
4 2
5 1
```




```output1
0
```




```output2
1
```




```output3
2
```




```output4
19
```




```output5
6
```



## Note

<p>In example $1$, Annie can travel to each spot directly and plant a potato with no energy required.</p><p>In example $2$, moving to $(1,0)$, Annie plants the second potato using $1$ energy. Next, she travels to $(1,1)$ and plants the first potato with $0$ energy.</p>
