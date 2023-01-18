## Description

<div><p>Slime and Orac are holding a turn-based game. In a big room, there are $n$ players sitting on the chairs, looking forward to a column and each of them is given a number: player $1$ sits in the front of the column, player $2$ sits directly behind him; player $3$ sits directly behind player $2$, and so on; player $n$ sits directly behind player $n-1$. Each player wears a hat that is either black or white. As each player faces forward, player $i$ knows the color of player $j$'s hat if and only if $i$ is larger than $j$.</p><p>At the start of each turn, Orac will tell <span class="tex-font-style-bf">whether there exists a player wearing a black hat in the room</span>.</p><p>After Orac speaks, if the player can uniquely identify the color of his hat, he will put his hat on the chair, stand up and leave the room. All players are smart, so if it is possible to understand the color of their hat using the obtained information during this and previous rounds, they will understand it.</p><p> In each turn, all players who know the color of their hats will leave at the same time in this turn, which means a player can only leave in the next turn if he gets to know the color of his hat only after someone left the room at this turn.</p><p>Note that when the player needs to leave, he will put the hat on the chair before leaving, so the players ahead of him still cannot see his hat. </p><p>The $i$-th player will know who exactly left the room among players $1,2,\ldots,i-1$, and how many players among $i+1,i+2,\ldots,n$ have left the room.</p><p>Slime stands outdoor. He watches the players walking out and records the numbers of the players and the time they get out. Unfortunately, Slime is so careless that he has only recorded some of the data, and this given data is in the format "<span class="tex-font-style-tt">player $x$ leaves in the $y$-th round</span>".</p><p>Slime asked you to tell him the color of each player's hat. If there are multiple solutions, you can find any of them.</p></div><div class="input-specification"><p>The first line contains a integer $n\ (1\le n\le 200\,000)$.</p><p>The second line contains $n$ integers $t_1,t_2,\dots,t_n\ (0\le t_i\le 10^{15})$. If $t_i=0$, then there are no data about player $i$; otherwise it means player $i$ leaves in the $t_i$-th round.</p><p>At least one solution exists for the given input. </p></div><div class="output-specification"><p>Print one binary string of $n$ characters. The $i$-th character of the string should be '<span class="tex-font-style-tt">1</span>' if player $i$ wears a black hat and should be '<span class="tex-font-style-tt">0</span>', otherwise. If there are multiple solutions, you can print any of them.</p></div>

## Input

<p>The first line contains a integer $n\ (1\le n\le 200\,000)$.</p><p>The second line contains $n$ integers $t_1,t_2,\dots,t_n\ (0\le t_i\le 10^{15})$. If $t_i=0$, then there are no data about player $i$; otherwise it means player $i$ leaves in the $t_i$-th round.</p><p>At least one solution exists for the given input. </p>

## Output

<p>Print one binary string of $n$ characters. The $i$-th character of the string should be '<span class="tex-font-style-tt">1</span>' if player $i$ wears a black hat and should be '<span class="tex-font-style-tt">0</span>', otherwise. If there are multiple solutions, you can print any of them.</p>





```input1
5
0 1 1 0 0
```




```input2
5
0 2 2 0 0
```




```input3
5
0 0 0 0 0
```




```input4
5
4 4 0 4 4
```




```output1
00000
```




```output2
00001
```




```output3
00000
```




```output4
00100
```



## Note

<p>In the first example, for the given solution, all the players wear white hats. In the first turn, Orac tells all the players that there are no players wearing a black hat, so each player knows that he is wearing a white hat, and he will leave in the first turn.</p><p>In the second example, for the given solution, the player $5$ wears a black hat, other players wear white hats. Orac tells all the players that there exists a player wearing a black hat, and player $5$ know that the other players are all wearing white hats, so he can infer that he is wearing a black hat; therefore he leaves in the first turn, other players leave in the second turn. Note that other players can infer that they are wearing white hats immediately after player $5$ leaves, but they have to wait for the next turn to leave according to the rule.</p><p>In the third example, there is no information about the game, so any output is correct.</p>
