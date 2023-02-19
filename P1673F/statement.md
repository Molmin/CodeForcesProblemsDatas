## Description

<div><p><span class="tex-font-style-it">This is an interactive problem.</span></p><p>A city has $n^2$ buildings divided into a grid of $n$ rows and $n$ columns. You need to build a road of some length $D(A,B)$ of your choice between each pair of adjacent by side buildings $A$ and $B$. Due to budget limitations and legal restrictions, the length of each road must be a positive integer and <span class="tex-font-style-bf">the total length of all roads should not exceed $48\,000$</span>.</p><p>There is a thief in the city who will start from the topmost, leftmost building (in the first row and the first column) and roam around the city, occasionally stealing artifacts from some of the buildings. He can move from one building to another adjacent building by travelling through the road which connects them.</p><p>You are unable to track down what buildings he visits and what path he follows to reach them. But there is one tracking mechanism in the city. The tracker is capable of storing a single integer $x$ which is initially $0$. Each time the thief travels from a building $A$ to another adjacent building $B$ through a road of length $D(A,B)$, the tracker changes $x$ to $x\oplus D(A,B)$. Each time the thief steals from a building, the tracker reports the value $x$ stored in it and resets it back to $0$.</p><p>It is known beforehand that the thief will steal in exactly $k$ buildings but you will know the values returned by the tracker only after the thefts actually happen. Your task is to choose the lengths of roads in such a way that no matter what strategy or routes the thief follows, you will be able to exactly tell the location of all the buildings where the thefts occurred from the values returned by the tracker.</p></div><div><h2>Interaction</h2><p>First read a single line containing two integers $n$ $(2\leq n\leq 32)$ and $k$ $(1\leq k\leq 1024)$ denoting the number of rows and number of thefts respectively.</p><p>Let's denote the $j$-th building in the $i$-th row by $B_{i,j}$.</p><p>Then print $n$ lines each containing $n-1$ integers. The $j$-th integer of the $i$-th line must be the value of $D(B_{i,j},B_{i,j+1})$.</p><p>Then print $n-1$ lines each containing $n$ integers. The $j$-th integer of the $i$-th line must be the value of $D(B_{i,j},B_{i+1,j})$.</p><p>Remember that the total length of the roads must not exceed $48\,000$.</p><p>Then answer $k$ queries. First read the value $x$ returned by the tracker. Then print two integers denoting the row number and column number of the building where the theft occurred. After that you will be able to answer the next query (if such exists).</p><p>After printing the answers do not forget to output end of line and flush the output buffer. Otherwise you will get the verdict <span class="tex-font-style-tt">Idleness limit exceeded</span>. To flush the buffer, use:</p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> Read documentation for other languages. </li></ul><p><span class="tex-font-style-bf">Hacks</span></p><p>You cannot make hacks in this problem.</p></div>





```input1
2 4



14

1

14

3
```




```output1
1
8
2 4

1 2

1 1

1 2

2 1
```



## Note

<p>For the sample test, $n=2$ and $k=4$.</p><p>You choose to build the roads of the following lengths:</p><center> <img class="tex-graphics" src="file://JcUYmeOE.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The thief follows the following strategy: </p><ol> <li> Start at $B_{1,1}$. </li><li> Move Right to $B_{1,2}$. </li><li> Move Down to $B_{2,2}$. </li><li> Move Left to $B_{2,1}$. </li><li> Move Up to $B_{1,1}$. </li><li> Move Right to $B_{1,2}$. </li><li> Steal from $B_{1,2}$. </li><li> Move Left to $B_{1,1}$. </li><li> Steal from $B_{1,1}$. </li><li> Move Down to $B_{2,1}$. </li><li> Move Right to $B_{2,2}$. </li><li> Move Up to $B_{1,2}$. </li><li> Steal from $B_{1,2}$. </li><li> Move Left to $B_{1,1}$. </li><li> Move Down to $B_{2,1}$. </li><li> Steal from $B_{2,1}$. </li></ol><p>The tracker responds in the following way: </p><ol> <li> Initialize $x=0$. </li><li> Change $x$ to $x\oplus 1=0\oplus1=1$. </li><li> Change $x$ to $x\oplus 4=1\oplus4=5$. </li><li> Change $x$ to $x\oplus 8=5\oplus8=13$. </li><li> Change $x$ to $x\oplus 2=13\oplus2=15$. </li><li> Change $x$ to $x\oplus 1=15\oplus1=14$. </li><li> Return $x=14$ and re-initialize $x=0$. </li><li> Change $x$ to $x\oplus 1=0\oplus1=1$. </li><li> Return $x=1$ and re-initialize $x=0$. </li><li> Change $x$ to $x\oplus 2=0\oplus2=2$. </li><li> Change $x$ to $x\oplus 8=2\oplus8=10$. </li><li> Change $x$ to $x\oplus 4=10\oplus4=14$. </li><li> Return $x=14$ and re-initialize $x=0$. </li><li> Change $x$ to $x\oplus 1=0\oplus1=1$. </li><li> Change $x$ to $x\oplus 2=1\oplus2=3$. </li><li> Return $x=3$ and re-initialize $x=0$. </li></ol>
