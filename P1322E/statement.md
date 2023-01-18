## Description

<div><p>Berland&nbsp;— is a huge country with diverse geography. One of the most famous natural attractions of Berland is the "Median mountain range". This mountain range is $n$ mountain peaks, located on one straight line and numbered in order of $1$ to $n$. The height of the $i$-th mountain top is $a_i$. </p><p>"Median mountain range" is famous for the so called <span class="tex-font-style-it">alignment of mountain peaks</span> happening to it every day. At the moment of alignment simultaneously for each mountain from $2$ to $n - 1$ its height becomes equal to the median height among it and two neighboring mountains. Formally, if before the alignment the heights were equal $b_i$, then after the alignment new heights $a_i$ are as follows: $a_1 = b_1$, $a_n = b_n$ and for all $i$ from $2$ to $n - 1$ $a_i = \texttt{median}(b_{i-1}, b_i, b_{i+1})$. The median of three integers is the second largest number among them. For example, $\texttt{median}(5,1,2) = 2$, and $\texttt{median}(4,2,4) = 4$.</p><p>Recently, Berland scientists have proved that whatever are the current heights of the mountains, the alignment process will stabilize sooner or later, i.e. at some point the altitude of the mountains won't changing after the alignment any more. The government of Berland wants to understand how soon it will happen, i.e. to find the value of $c$&nbsp;— how many alignments will occur, which will change the height of at least one mountain. Also, the government of Berland needs to determine the heights of the mountains after $c$ alignments, that is, find out what heights of the mountains stay forever. Help scientists solve this important problem!</p></div><div class="input-specification"><p>The first line contains integers $n$ ($1 \le n \le 500\,000$)&nbsp;— the number of mountains.</p><p>The second line contains integers $a_1, a_2, a_3, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— current heights of the mountains.</p></div><div class="output-specification"><p>In the first line print $c$&nbsp;— the number of alignments, which change the height of at least one mountain.</p><p>In the second line print $n$ integers&nbsp;— the final heights of the mountains after $c$ alignments.</p></div>

## Input

<p>The first line contains integers $n$ ($1 \le n \le 500\,000$)&nbsp;— the number of mountains.</p><p>The second line contains integers $a_1, a_2, a_3, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— current heights of the mountains.</p>

## Output

<p>In the first line print $c$&nbsp;— the number of alignments, which change the height of at least one mountain.</p><p>In the second line print $n$ integers&nbsp;— the final heights of the mountains after $c$ alignments.</p>





```input1
5
1 2 1 2 1
```




```input2
6
1 3 2 5 4 6
```




```input3
6
1 1 2 2 1 1
```




```output1
2
1 1 1 1 1
```




```output2
1
1 2 3 4 5 6
```




```output3
0
1 1 2 2 1 1
```



## Note

<p>In the first example, the heights of the mountains at index $1$ and $5$ never change. Since the median of $1$, $2$, $1$ is $1$, the second and the fourth mountains will have height 1 after the first alignment, and since the median of $2$, $1$, $2$ is $2$, the third mountain will have height 2 after the first alignment. This way, after one alignment the heights are $1$, $1$, $2$, $1$, $1$. After the second alignment the heights change into $1$, $1$, $1$, $1$, $1$ and never change from now on, so there are only $2$ alignments changing the mountain heights.</p><p>In the third examples the alignment doesn't change any mountain height, so the number of alignments changing any height is $0$.</p>
