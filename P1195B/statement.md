## Description

<div><p>Each evening after the dinner the SIS's students gather together to play the game of Sport Mafia. </p><p>For the tournament, Alya puts candies into the box, which will serve as a prize for a winner. To do that, she performs $n$ actions. The first action performed is to put a single candy into the box. For each of the remaining moves she can choose from two options:</p><ul> <li> the first option, in case the box contains at least one candy, is to take <span class="tex-font-style-bf">exactly one candy out and eat it</span>. This way the number of candies in the box decreased by $1$; </li><li> the second option is to put candies in the box. In this case, Alya will put $1$ more candy, than she put in the previous time. </li></ul><p>Thus, if the box is empty, then it can only use the second option.</p><p>For example, one possible sequence of Alya's actions look as follows:</p><ul> <li> put one candy into the box; </li><li> put two candies into the box; </li><li> eat one candy from the box; </li><li> eat one candy from the box; </li><li> put three candies into the box; </li><li> eat one candy from the box; </li><li> put four candies into the box; </li><li> eat one candy from the box; </li><li> put five candies into the box; </li></ul><p>This way she will perform $9$ actions, the number of candies at the end will be $11$, while Alya will eat $4$ candies in total.</p><p>You know the total number of actions $n$ and the number of candies at the end $k$. You need to find the total number of sweets Alya ate. That is the number of moves of the first option. It's guaranteed, that for the given $n$ and $k$ the answer always exists.</p><p>Please note, that during an action of the first option, Alya takes out and eats exactly one candy.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($1 \le n \le 10^9$; $0 \le k \le 10^9$)&nbsp;— the total number of moves and the number of candies in the box at the end. </p><p>It's guaranteed, that for the given $n$ and $k$ the answer exists.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the number of candies, which Alya ate. Please note, that in this problem there aren't multiple possible answers&nbsp;— the answer is unique for any input data. </p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($1 \le n \le 10^9$; $0 \le k \le 10^9$)&nbsp;— the total number of moves and the number of candies in the box at the end. </p><p>It's guaranteed, that for the given $n$ and $k$ the answer exists.</p>

## Output

<p>Print a single integer&nbsp;— the number of candies, which Alya ate. Please note, that in this problem there aren't multiple possible answers&nbsp;— the answer is unique for any input data. </p>





```input1
1 1
```




```input2
9 11
```




```input3
5 0
```




```input4
3 2
```




```output1
0
```




```output2
4
```




```output3
3
```




```output4
1
```



## Note

<p>In the first example, Alya has made one move only. According to the statement, the first move is always putting one candy in the box. Hence Alya ate $0$ candies.</p><p>In the second example the possible sequence of Alya's actions looks as follows: </p><ul> <li> put $1$ candy, </li><li> put $2$ candies, </li><li> eat a candy, </li><li> eat a candy, </li><li> put $3$ candies, </li><li> eat a candy, </li><li> put $4$ candies, </li><li> eat a candy, </li><li> put $5$ candies. </li></ul> <p>This way, she will make exactly $n=9$ actions and in the end the box will contain $1+2-1-1+3-1+4-1+5=11$ candies. The answer is $4$, since she ate $4$ candies in total.</p>
