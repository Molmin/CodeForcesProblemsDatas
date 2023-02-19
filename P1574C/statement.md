## Description

<div><p>Recently, Petya learned about a new game "Slay the Dragon". As the name suggests, the player will have to fight with dragons. To defeat a dragon, you have to kill it and defend your castle. To do this, the player has a squad of $n$ heroes, the strength of the $i$-th hero is equal to $a_i$.</p><p>According to the rules of the game, exactly one hero should go kill the dragon, all the others will defend the castle. If the dragon's defense is equal to $x$, then you have to send a hero with a strength of at least $x$ to kill it. If the dragon's attack power is $y$, then the total strength of the heroes defending the castle should be at least $y$.</p><p>The player can increase the strength of any hero by $1$ for one gold coin. This operation can be done any number of times.</p><p>There are $m$ dragons in the game, the $i$-th of them has defense equal to $x_i$ and attack power equal to $y_i$. Petya was wondering what is the minimum number of coins he needs to spend to defeat the $i$-th dragon.</p><p>Note that the task is solved <span class="tex-font-style-bf">independently for each dragon</span> (improvements are not saved).</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$)&nbsp;— number of heroes.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^{12}$), where $a_i$ is the strength of the $i$-th hero.</p><p>The third line contains a single integer $m$ ($1 \le m \le 2 \cdot 10^5$)&nbsp;— the number of dragons.</p><p>The next $m$ lines contain two integers each, $x_i$ and $y_i$ ($1 \le x_i \le 10^{12}; 1 \le y_i \le 10^{18}$)&nbsp;— defense and attack power of the $i$-th dragon.</p></div><div class="output-specification"><p>Print $m$ lines, $i$-th of which contains a single integer&nbsp;— the minimum number of coins that should be spent to defeat the $i$-th dragon.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$)&nbsp;— number of heroes.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^{12}$), where $a_i$ is the strength of the $i$-th hero.</p><p>The third line contains a single integer $m$ ($1 \le m \le 2 \cdot 10^5$)&nbsp;— the number of dragons.</p><p>The next $m$ lines contain two integers each, $x_i$ and $y_i$ ($1 \le x_i \le 10^{12}; 1 \le y_i \le 10^{18}$)&nbsp;— defense and attack power of the $i$-th dragon.</p>

## Output

<p>Print $m$ lines, $i$-th of which contains a single integer&nbsp;— the minimum number of coins that should be spent to defeat the $i$-th dragon.</p>





```input1
4
3 6 2 3
5
3 12
7 9
4 14
1 10
8 7
```




```output1
1
2
4
0
2
```



## Note

<p>To defeat the first dragon, you can increase the strength of the third hero by $1$, then the strength of the heroes will be equal to $[3, 6, 3, 3]$. To kill the dragon, you can choose the first hero.</p><p>To defeat the second dragon, you can increase the forces of the second and third heroes by $1$, then the strength of the heroes will be equal to $[3, 7, 3, 3]$. To kill the dragon, you can choose a second hero.</p><p>To defeat the third dragon, you can increase the strength of all the heroes by $1$, then the strength of the heroes will be equal to $[4, 7, 3, 4]$. To kill the dragon, you can choose a fourth hero.</p><p>To defeat the fourth dragon, you don't need to improve the heroes and choose a third hero to kill the dragon.</p><p>To defeat the fifth dragon, you can increase the strength of the second hero by $2$, then the strength of the heroes will be equal to $[3, 8, 2, 3]$. To kill the dragon, you can choose a second hero.</p>
