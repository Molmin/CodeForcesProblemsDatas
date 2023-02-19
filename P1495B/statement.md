## Description

<div><p>On a weekend, Qingshan suggests that she and her friend Daniel go hiking. Unfortunately, they are busy high school students, so they can only go hiking on scratch paper.</p><p>A permutation $p$ is written from left to right on the paper. First Qingshan chooses an integer index $x$ ($1\le x\le n$) and tells it to Daniel. After that, Daniel chooses another integer index $y$ ($1\le y\le n$, $y \ne x$).</p><p>The game progresses turn by turn and as usual, Qingshan moves first. The rules follow: </p><ul> <li> If it is Qingshan's turn, Qingshan must change $x$ to such an index $x'$ that $1\le x'\le n$, $|x'-x|=1$, $x'\ne y$, and $p_{x'}&lt;p_x$ at the same time. </li><li> If it is Daniel's turn, Daniel must change $y$ to such an index $y'$ that $1\le y'\le n$, $|y'-y|=1$, $y'\ne x$, and $p_{y'}&gt;p_y$ at the same time. </li></ul><p>The person who can't make her or his move loses, and the other wins. You, as Qingshan's fan, are asked to calculate the number of possible $x$ to make Qingshan win in the case both players play optimally.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2\le n\le 10^5$)&nbsp;— the length of the permutation.</p><p>The second line contains $n$ distinct integers $p_1,p_2,\dots,p_n$ ($1\le p_i\le n$)&nbsp;— the permutation.</p></div><div class="output-specification"><p>Print the number of possible values of $x$ that Qingshan can choose to make her win.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2\le n\le 10^5$)&nbsp;— the length of the permutation.</p><p>The second line contains $n$ distinct integers $p_1,p_2,\dots,p_n$ ($1\le p_i\le n$)&nbsp;— the permutation.</p>

## Output

<p>Print the number of possible values of $x$ that Qingshan can choose to make her win.</p>





```input1
5
1 2 5 4 3
```




```input2
7
1 2 4 6 5 3 7
```




```output1
1
```




```output2
0
```



## Note

<p>In the first test case, Qingshan can only choose $x=3$ to win, so the answer is $1$.</p><p>In the second test case, if Qingshan will choose $x=4$, Daniel can choose $y=1$. In the first turn (Qingshan's) Qingshan chooses $x'=3$ and changes $x$ to $3$. In the second turn (Daniel's) Daniel chooses $y'=2$ and changes $y$ to $2$. Qingshan can't choose $x'=2$ because $y=2$ at this time. Then Qingshan loses.</p>
