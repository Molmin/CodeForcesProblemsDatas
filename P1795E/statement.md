## Description

<div><p>You are playing yet another game where you kill monsters using magic spells. There are $n$ cells in the row, numbered from $1$ to $n$. Initially, the $i$-th cell contains the $i$-th monster with $h_i$ health.</p><p>You have a basic spell that costs $1$ MP and deals $1$ damage to the monster you choose. You can cast it any number of times. Also, you have a special scroll with "Explosion" spell you can use only once. You want to finish killing monsters with explosion, that's why you, firstly, cast the basic spell several times (possibly, zero), and then after that, you cast one "Explosion".</p><p>How does "Explosion" spell work? Firstly, you choose the power of the spell: if you pour $x$ MP into it, "Explosion" will deal $x$ damage. Secondly, you choose some monster $i$, which will be targeted by the spell. That's what happens next: </p><ul> <li> if its <span class="tex-font-style-bf">current</span> health $h_i &gt; x$, then he stays alive with health decreased by $x$; </li><li> if $h_i \le x$, the $i$-th monster dies with an explosion that deals $h_i - 1$ damage to monsters in the neighboring cells $i - 1$ and $i + 1$, if these cells exist and monsters inside are still alive; </li><li> if the damage dealt by the explosion is enough to kill the monster $i - 1$ (or $i + 1$), i.&nbsp;e. the current $h_{i - 1} \le h_i - 1$ (or $h_{i + 1} \le h_i - 1$), then that monster also dies creating a secondary explosion of power $h_{i-1} - 1$ (or $h_{i+1} - 1$) that may deals damage to their neighbors, and so on, until the explosions end. </li></ul><p>Your goal is to kill all the remaining monsters with those "chaining" explosions, that's why you need a basic spell to decrease $h_i$ of some monsters or even kill them beforehand (monsters die when their current health $h_i$ becomes less or equal to zero). Note that monsters don't move between cells, so, for example, monsters $i$ and $i + 2$ will never become neighbors.</p><p>What is the minimum total MP you need to kill all monsters in the way you want? The total MP is counted as the sum of the number of basic spells you cast and the power $x$ of explosion scroll you've chosen.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains the single integer $n$ ($1 \le n \le 3 \cdot 10^5$)&nbsp;— the number of cells in the row, i.&nbsp;e. the number of monsters.</p><p>The second line of each test case contains $n$ integers $h_1, h_2, \dots, h_n$ ($1 \le h_i \le 10^6$)&nbsp;— the initial health of the monsters.</p><p>It's guaranteed that the sum of $n$ over all test cases doesn't exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print one integer&nbsp;— the minimum total MP you need to kill all monsters by finishing them with explosion.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains the single integer $n$ ($1 \le n \le 3 \cdot 10^5$)&nbsp;— the number of cells in the row, i.&nbsp;e. the number of monsters.</p><p>The second line of each test case contains $n$ integers $h_1, h_2, \dots, h_n$ ($1 \le h_i \le 10^6$)&nbsp;— the initial health of the monsters.</p><p>It's guaranteed that the sum of $n$ over all test cases doesn't exceed $3 \cdot 10^5$.</p>

## Output

<p>For each test case, print one integer&nbsp;— the minimum total MP you need to kill all monsters by finishing them with explosion.</p>





```input1|2,3,6,7,10,11
5
3
1 1 1
4
4 1 2 1
4
5 10 15 10
1
42
9
1 2 3 2 2 2 3 2 1
```




```output1
3
6
15
42
12
```



## Note

<p>In the first test case, you can, for example, use basic spell on monsters $1$ and $2$ (once per monster) to kill them. After that, you cast "Explosion" of power $x = 1$ on monster $3$ to kill it. The total MP you need is $2 + 1 = 3$.</p><p>In the second test case, it's optimal to cast basic spell $4$ times onto monster $1$ to kill it. After that, you can cast "Explosion" of power $x = 2$ onto monster $3$. It dies, creating an explosion of power $1$ that kills monsters $2$ and $4$. The total MP you need is $4 + 2 = 6$.</p><p>In the third test case, you cast "Explosion" of power $15$ onto monster $3$. Explosion of the $3$-rd monster (of power $14$) kills monsters $2$ and $4$. Secondary explosion of monster $2$ (of power $9$) kills monster $1$.</p>
