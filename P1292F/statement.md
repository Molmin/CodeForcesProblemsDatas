## Description

<div><div class="epigraph"><div class="epigraph-text"><a href="https://soundcloud.com/hanatsuka/sihanatsuka-ember"><span class="tex-font-style-it">SIHanatsuka - EMber</span></a></div></div> <div class="epigraph"><div class="epigraph-text"><a href="https://soundcloud.com/hanatsuka/sihanatsuka-atonement"><span class="tex-font-style-it">SIHanatsuka - ATONEMENT</span></a></div></div><p>Back in time, the seven-year-old Nora used to play lots of games with her creation ROBO_Head-02, both to have fun and enhance his abilities.</p><p>One day, Nora's adoptive father, Phoenix Wyle, brought Nora $n$ boxes of toys. Before unpacking, Nora decided to make a fun game for ROBO.</p><p>She labelled all $n$ boxes with $n$ distinct integers $a_1, a_2, \ldots, a_n$ and asked ROBO to do the following action several (possibly zero) times:</p><ul> <li> Pick three distinct indices $i$, $j$ and $k$, such that $a_i \mid a_j$ and $a_i \mid a_k$. In other words, $a_i$ divides both $a_j$ and $a_k$, that is $a_j \bmod a_i = 0$, $a_k \bmod a_i = 0$. </li><li> After choosing, Nora will give the $k$-th box to ROBO, and he will place it on top of the box pile at his side. Initially, the pile is empty. </li><li> After doing so, the box $k$ becomes unavailable for any further actions. </li></ul><p>Being amused after nine different tries of the game, Nora asked ROBO to calculate the number of possible different piles having the <span class="tex-font-style-bf">largest</span> amount of boxes in them. Two piles are considered different if there exists a position where those two piles have different boxes.</p><p>Since ROBO was still in his infant stages, and Nora was still too young to concentrate for a long time, both fell asleep before finding the final answer. Can you help them?</p><p>As the number of such piles can be very large, you should print the answer modulo $10^9 + 7$.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($3 \le n \le 60$), denoting the number of boxes.</p><p>The second line contains $n$ distinct integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 60$), where $a_i$ is the label of the $i$-th box.</p></div><div class="output-specification"><p>Print the number of distinct piles having the maximum number of boxes that ROBO_Head can have, modulo $10^9 + 7$.</p></div>

## Input

<p>The first line contains an integer $n$ ($3 \le n \le 60$), denoting the number of boxes.</p><p>The second line contains $n$ distinct integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 60$), where $a_i$ is the label of the $i$-th box.</p>

## Output

<p>Print the number of distinct piles having the maximum number of boxes that ROBO_Head can have, modulo $10^9 + 7$.</p>





```input1
3
2 6 8
```




```input2
5
2 3 4 9 12
```




```input3
4
5 7 2 9
```




```output1
2
```




```output2
4
```




```output3
1
```



## Note

<p>Let's illustrate the box pile as a sequence $b$, with the pile's bottommost box being at the leftmost position.</p><p>In the first example, there are $2$ distinct piles possible: </p><ul> <li> $b = [6]$ ($[2, \mathbf{6}, 8] \xrightarrow{(1, 3, 2)} [2, 8]$) </li><li> $b = [8]$ ($[2, 6, \mathbf{8}] \xrightarrow{(1, 2, 3)} [2, 6]$) </li></ul><p>In the second example, there are $4$ distinct piles possible: </p><ul> <li> $b = [9, 12]$ ($[2, 3, 4, \mathbf{9}, 12] \xrightarrow{(2, 5, 4)} [2, 3, 4, \mathbf{12}] \xrightarrow{(1, 3, 4)} [2, 3, 4]$) </li><li> $b = [4, 12]$ ($[2, 3, \mathbf{4}, 9, 12] \xrightarrow{(1, 5, 3)} [2, 3, 9, \mathbf{12}] \xrightarrow{(2, 3, 4)} [2, 3, 9]$) </li><li> $b = [4, 9]$ ($[2, 3, \mathbf{4}, 9, 12] \xrightarrow{(1, 5, 3)} [2, 3, \mathbf{9}, 12] \xrightarrow{(2, 4, 3)} [2, 3, 12]$) </li><li> $b = [9, 4]$ ($[2, 3, 4, \mathbf{9}, 12] \xrightarrow{(2, 5, 4)} [2, 3, \mathbf{4}, 12] \xrightarrow{(1, 4, 3)} [2, 3, 12]$) </li></ul><p>In the third sequence, ROBO can do nothing at all. Therefore, there is only $1$ valid pile, and that pile is empty.</p>
