## Description

<div><p>Sasha and Dima want to buy two $n$-tier cakes. Each cake should consist of $n$ different tiers: from the size of $1$ to the size of $n$. Tiers should go in order from the smallest to the biggest (from top to bottom).</p><p>They live on the same street, there are $2 \cdot n$ houses in a row from left to right. Each house has a pastry shop where you can buy a cake tier. Unfortunately, in each pastry shop you can buy only one tier of only one specific size: in the $i$-th house you can buy a tier of the size $a_i$ ($1 \le a_i \le n$).</p><p>Since the guys carry already purchased tiers, and it is impossible to insert a new tier in the middle of the cake, they agreed to buy tiers from the smallest to the biggest. That is, each of them buys tiers in order: $1$, then $2$, then $3$ and so on up to $n$.</p><p>Initially, Sasha and Dima are located near the first (leftmost) house. Output the minimum distance that they will have to walk in total to buy both cakes. The distance between any two neighboring houses is exactly $1$.</p></div><div class="input-specification"><p>The first line of the input contains an integer number $n$ — the number of tiers in each cake ($1 \le n \le 10^5$).</p><p>The second line contains $2 \cdot n$ integers $a_1, a_2, \dots, a_{2n}$ ($1 \le a_i \le n$), where $a_i$ is equal to the size of the tier, which can be bought in the $i$-th house. Remember that in each house you can buy only one tier. It is guaranteed that every number from $1$ to $n$ occurs in $a$ exactly two times.</p></div><div class="output-specification"><p>Print one number &nbsp;— the minimum distance that the guys have to walk in total to buy both cakes. Guys can be near same house at the same time. They begin near the first (leftmost) house. Each of the guys should buy $n$ tiers in ascending order of their sizes.</p></div>

## Input

<p>The first line of the input contains an integer number $n$ — the number of tiers in each cake ($1 \le n \le 10^5$).</p><p>The second line contains $2 \cdot n$ integers $a_1, a_2, \dots, a_{2n}$ ($1 \le a_i \le n$), where $a_i$ is equal to the size of the tier, which can be bought in the $i$-th house. Remember that in each house you can buy only one tier. It is guaranteed that every number from $1$ to $n$ occurs in $a$ exactly two times.</p>

## Output

<p>Print one number &nbsp;— the minimum distance that the guys have to walk in total to buy both cakes. Guys can be near same house at the same time. They begin near the first (leftmost) house. Each of the guys should buy $n$ tiers in ascending order of their sizes.</p>





```input1
3
1 1 2 2 3 3
```




```input2
2
2 1 1 2
```




```input3
4
4 1 3 2 2 3 1 4
```




```output1
9
```




```output2
5
```




```output3
17
```



## Note

<p>In the first example, the possible optimal sequence of actions is:</p><ul> <li> Sasha buys a tier of size $1$ near the $1$-st house ($a_1=1$); </li><li> Dima goes to the house $2$; </li><li> Dima buys a tier of size $1$ near the $2$-nd house ($a_2=1$); </li><li> Sasha goes to the house $4$; </li><li> Sasha buys a tier of size $2$ near the $4$-th house ($a_4=2$); </li><li> Sasha goes to the house $5$; </li><li> Sasha buys a tier of size $3$ near the $5$-th house ($a_5=3$); </li><li> Dima goes to the house $3$; </li><li> Dima buys a tier of size $2$ near the $3$-rd house ($a_3=2$); </li><li> Dima goes to the house $6$; </li><li> Dima buys a tier of size $3$ near the $6$-th house ($a_6=3$). </li></ul><p>So, Sasha goes the distance $3+1=4$, and Dima goes the distance $1+1+3=5$. In total, they cover a distance of $4+5=9$. You can make sure that with any other sequence of actions they will walk no less distance.</p>
