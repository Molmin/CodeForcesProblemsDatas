## Description

<div><p>Ivan is playing yet another roguelike computer game. He controls a single hero in the game. The hero has $n$ equipment slots. There is a list of $c_i$ items for the $i$-th slot, the $j$-th of them increases the hero strength by $a_{i,j}$. The items for each slot are pairwise distinct and are listed in the increasing order of their strength increase. So, $a_{i,1} &lt; a_{i,2} &lt; \dots &lt; a_{i,c_i}$.</p><p>For each slot Ivan chooses exactly one item. Let the chosen item for the $i$-th slot be the $b_i$-th item in the corresponding list. The sequence of choices $[b_1, b_2, \dots, b_n]$ is called <span class="tex-font-style-it">a build</span>.</p><p>The strength of a build is the sum of the strength increases of the items in it. Some builds are banned from the game. There is a list of $m$ pairwise distinct banned builds. It's guaranteed that there's at least one build that's not banned.</p><p>What is the build with the maximum strength that is not banned from the game? If there are multiple builds with maximum strength, print any of them.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 10$)&nbsp;— the number of equipment slots.</p><p>The $i$-th of the next $n$ lines contains the description of the items for the $i$-th slot. First, one integer $c_i$ ($1 \le c_i \le 2 \cdot 10^5$)&nbsp;— the number of items for the $i$-th slot. Then $c_i$ integers $a_{i,1}, a_{i,2}, \dots, a_{i,c_i}$ ($1 \le a_{i,1} &lt; a_{i,2} &lt; \dots &lt; a_{i,c_i} \le 10^8$).</p><p>The sum of $c_i$ doesn't exceed $2 \cdot 10^5$.</p><p>The next line contains a single integer $m$ ($0 \le m \le 10^5$)&nbsp;— the number of banned builds.</p><p>Each of the next $m$ lines contains a description of a banned build&nbsp;— a sequence of $n$ integers $b_1, b_2, \dots, b_n$ ($1 \le b_i \le c_i$).</p><p>The builds are pairwise distinct, and there's at least one build that's not banned.</p></div><div class="output-specification"><p>Print the build with the maximum strength that is not banned from the game. If there are multiple builds with maximum strength, print any of them.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 10$)&nbsp;— the number of equipment slots.</p><p>The $i$-th of the next $n$ lines contains the description of the items for the $i$-th slot. First, one integer $c_i$ ($1 \le c_i \le 2 \cdot 10^5$)&nbsp;— the number of items for the $i$-th slot. Then $c_i$ integers $a_{i,1}, a_{i,2}, \dots, a_{i,c_i}$ ($1 \le a_{i,1} &lt; a_{i,2} &lt; \dots &lt; a_{i,c_i} \le 10^8$).</p><p>The sum of $c_i$ doesn't exceed $2 \cdot 10^5$.</p><p>The next line contains a single integer $m$ ($0 \le m \le 10^5$)&nbsp;— the number of banned builds.</p><p>Each of the next $m$ lines contains a description of a banned build&nbsp;— a sequence of $n$ integers $b_1, b_2, \dots, b_n$ ($1 \le b_i \le c_i$).</p><p>The builds are pairwise distinct, and there's at least one build that's not banned.</p>

## Output

<p>Print the build with the maximum strength that is not banned from the game. If there are multiple builds with maximum strength, print any of them.</p>





```input1
3
3 1 2 3
2 1 5
3 2 4 6
2
3 2 3
3 2 2
```




```input2
3
3 1 2 3
2 1 5
3 2 4 6
2
3 2 3
2 2 3
```




```input3
3
3 1 2 3
2 1 5
3 2 4 6
2
3 2 3
2 2 3
```




```input4
4
1 10
1 4
1 7
1 3
0
```




```output1
2 2 3
```




```output2
1 2 3
```




```output3
3 2 2
```




```output4
1 1 1 1
```


