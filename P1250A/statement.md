## Description

<div><p>Polycarp recently signed up to a new social network Berstagram. He immediately published $n$ posts there. He assigned numbers from $1$ to $n$ to all posts and published them one by one. So, just after publishing Polycarp's news feed contained posts from $1$ to $n$ — the highest post had number $1$, the next one had number $2$, ..., the lowest post had number $n$.</p><p>After that he wrote down all likes from his friends. Likes were coming consecutively from the $1$-st one till the $m$-th one. You are given a sequence $a_1, a_2, \dots, a_m$ ($1 \le a_j \le n$), where $a_j$ is the post that received the $j$-th like.</p><p>News feed in Berstagram works in the following manner. Let's assume the $j$-th like was given to post $a_j$. If this post is not the highest (first) one then it changes its position with the one above. If $a_j$ is the highest post nothing changes. </p><p>For example, if $n=3$, $m=5$ and $a=[3,2,1,3,3]$, then Polycarp's news feed had the following states:</p><ul> <li> before the first like: $[1, 2, 3]$; </li><li> after the first like: $[1, 3, 2]$; </li><li> after the second like: $[1, 2, 3]$; </li><li> after the third like: $[1, 2, 3]$; </li><li> after the fourth like: $[1, 3, 2]$; </li><li> after the fifth like: $[3, 1, 2]$. </li></ul><p>Polycarp wants to know the highest (minimum) and the lowest (maximum) positions for each post. Polycarp considers all moments of time, including the moment "before all likes".</p></div><div class="input-specification"><p>The first line contains two integer numbers $n$ and $m$ ($1 \le n \le 10^5$, $1 \le m \le 4 \cdot10^5$) — number of posts and number of likes. </p><p>The second line contains integers $a_1, a_2, \dots, a_m$ ($1 \le a_j \le n$), where $a_j$ is the post that received the $j$-th like.</p></div><div class="output-specification"><p>Print $n$ pairs of integer numbers. The $i$-th line should contain the highest (minimum) and the lowest (maximum) positions of the $i$-th post. You should take into account positions at all moments of time: before all likes, after each like and after all likes. Positions are numbered from $1$ (highest) to $n$ (lowest).</p></div>

## Input

<p>The first line contains two integer numbers $n$ and $m$ ($1 \le n \le 10^5$, $1 \le m \le 4 \cdot10^5$) — number of posts and number of likes. </p><p>The second line contains integers $a_1, a_2, \dots, a_m$ ($1 \le a_j \le n$), where $a_j$ is the post that received the $j$-th like.</p>

## Output

<p>Print $n$ pairs of integer numbers. The $i$-th line should contain the highest (minimum) and the lowest (maximum) positions of the $i$-th post. You should take into account positions at all moments of time: before all likes, after each like and after all likes. Positions are numbered from $1$ (highest) to $n$ (lowest).</p>





```input1
3 5
3 2 1 3 3
```




```input2
10 6
7 3 5 7 3 6
```




```output1
1 2
2 3
1 3
```




```output2
1 2
2 3
1 3
4 7
4 5
6 7
5 7
8 8
9 9
10 10
```


