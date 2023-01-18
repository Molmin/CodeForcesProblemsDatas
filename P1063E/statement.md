## Description

<div><p>Oleg came to see the maze of mirrors. The maze is a $n$ by $n$ room in which each cell is either empty or contains a mirror connecting opposite corners of this cell. Mirrors in this maze reflect light in a perfect way, which causes the interesting visual effects and contributes to the loss of orientation in the maze.</p><p>Oleg is a person of curious nature, so he decided to install $n$ lasers facing internal of the maze on the south wall of the maze. On the north wall of the maze, Oleg installed $n$ receivers, also facing internal of the maze. Let's number lasers and receivers from west to east with distinct integers from $1$ to $n$. Each laser sends a beam of some specific kind and receiver with number $a_i$ should receive the beam sent from laser number $i$. Since two lasers' beams can't come to the same receiver, these numbers form a <span class="tex-font-style-it">permutation</span>&nbsp;— each of the receiver numbers occurs exactly once.</p><p>You came to the maze together with Oleg. Help him to place the mirrors in the initially empty maze so that the maximum number of lasers' beams will come to the receivers they should. There are no mirrors outside the maze, so if the laser beam leaves the maze, it will not be able to go back.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 1000$)&nbsp;— the size of the maze.</p><p>The second line contains a permutation of $n$ integers $a_i$ ($1 \le a_i \le n$), where $a_i$ defines the number of the receiver, to which the beam from $i$-th laser should come.</p></div><div class="output-specification"><p>In the first line print the maximum possible number of laser beams, which can come to the receivers they should.</p><p>In the next $n$ lines of length $n$ print the arrangement of mirrors, causing such number of laser beams to come where they should. If the corresponding cell is empty, print "<span class="tex-font-style-tt">.</span>", otherwise print "<span class="tex-font-style-tt">/</span>" or "<span class="tex-font-style-tt">\</span>", depending on the orientation of the mirror.</p><p>In your output north should be above, south should be below, and west and east should be on left and on the right respectively.</p><p>It is allowed for laser beams to come not to the receivers they correspond to, but they are not counted in the answer.</p><p>If there are multiple arrangements of mirrors leading to the optimal answer&nbsp;— print any of them.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 1000$)&nbsp;— the size of the maze.</p><p>The second line contains a permutation of $n$ integers $a_i$ ($1 \le a_i \le n$), where $a_i$ defines the number of the receiver, to which the beam from $i$-th laser should come.</p>

## Output

<p>In the first line print the maximum possible number of laser beams, which can come to the receivers they should.</p><p>In the next $n$ lines of length $n$ print the arrangement of mirrors, causing such number of laser beams to come where they should. If the corresponding cell is empty, print "<span class="tex-font-style-tt">.</span>", otherwise print "<span class="tex-font-style-tt">/</span>" or "<span class="tex-font-style-tt">\</span>", depending on the orientation of the mirror.</p><p>In your output north should be above, south should be below, and west and east should be on left and on the right respectively.</p><p>It is allowed for laser beams to come not to the receivers they correspond to, but they are not counted in the answer.</p><p>If there are multiple arrangements of mirrors leading to the optimal answer&nbsp;— print any of them.</p>





```input1
4
4 1 3 2

```




```output1
3
.\..
\\..
/../
...\

```



## Note

<p>The picture illustrates the arrangements of the mirrors in the first example.</p><center> <img class="tex-graphics" src="file://5mMp4vNM.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
