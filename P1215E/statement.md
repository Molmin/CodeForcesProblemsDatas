## Description

<div><p>Monocarp has arranged $n$ colored marbles in a row. The color of the $i$-th marble is $a_i$. Monocarp likes ordered things, so he wants to rearrange marbles in such a way that all marbles of the same color form a contiguos segment (and there is only one such segment for each color). </p><p>In other words, Monocarp wants to rearrange marbles so that, for every color $j$, if the leftmost marble of color $j$ is $l$-th in the row, and the rightmost marble of this color has position $r$ in the row, then every marble from $l$ to $r$ has color $j$.</p><p>To achieve his goal, Monocarp can do the following operation any number of times: choose two neighbouring marbles, and swap them.</p><p>You have to calculate the minimum number of operations Monocarp has to perform to rearrange the marbles. Note that the order of segments of marbles having equal color does not matter, it is only required that, for every color, all the marbles of this color form exactly one contiguous segment.</p></div><div class="input-specification"><p>The first line contains one integer $n$ $(2 \le n \le 4 \cdot 10^5)$ — the number of marbles.</p><p>The second line contains an integer sequence $a_1, a_2, \dots, a_n$ $(1 \le a_i \le 20)$, where $a_i$ is the color of the $i$-th marble.</p></div><div class="output-specification"><p>Print the minimum number of operations Monocarp has to perform to achieve his goal.</p></div>

## Input

<p>The first line contains one integer $n$ $(2 \le n \le 4 \cdot 10^5)$ — the number of marbles.</p><p>The second line contains an integer sequence $a_1, a_2, \dots, a_n$ $(1 \le a_i \le 20)$, where $a_i$ is the color of the $i$-th marble.</p>

## Output

<p>Print the minimum number of operations Monocarp has to perform to achieve his goal.</p>





```input1
7
3 4 2 3 4 2 2
```




```input2
5
20 1 14 10 2
```




```input3
13
5 5 4 4 3 5 7 6 5 4 4 6 5
```




```output1
3
```




```output2
0
```




```output3
21
```



## Note

<p>In the first example three operations are enough. Firstly, Monocarp should swap the third and the fourth marbles, so the sequence of colors is $[3, 4, 3, 2, 4, 2, 2]$. Then Monocarp should swap the second and the third marbles, so the sequence is $[3, 3, 4, 2, 4, 2, 2]$. And finally, Monocarp should swap the fourth and the fifth marbles, so the sequence is $[3, 3, 4, 4, 2, 2, 2]$. </p><p>In the second example there's no need to perform any operations.</p>
