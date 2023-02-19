## Description

<div><p>We play a game with $n$ dots on a number line.</p><p>The initial coordinate of the $i$-th dot is $x_i$. These coordinates are distinct. Every dot starts moving simultaneously with the same constant speed.</p><p>Each dot moves in the direction of the closest dot (different from itself) until it meets another dot. In the case of a tie, it goes to the left. Two dots meet if they are in the same coordinate, after that, they stop moving.</p><p>After enough time, every dot stops moving. The result of a game is the number of distinct coordinates where the dots stop.</p><p>Because this game is too easy, calculate the sum of results when we play the game for every subset of the given $n$ dots that has at least two dots. As the result can be very large, print the sum modulo $10^9+7$.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($2 \leq n \leq 3000$).</p><p>The next line contains $n$ integers $x_1, x_2, \ldots, x_n$ ($1 \leq x_1 &lt; x_2 &lt; \ldots &lt; x_n \leq 10^9$), where $x_i$ represents the initial coordinate of $i$-th dot.</p></div><div class="output-specification"><p>Print the sum of results modulo $10^9+7$.</p></div>

## Input

<p>The first line contains one integer $n$ ($2 \leq n \leq 3000$).</p><p>The next line contains $n$ integers $x_1, x_2, \ldots, x_n$ ($1 \leq x_1 &lt; x_2 &lt; \ldots &lt; x_n \leq 10^9$), where $x_i$ represents the initial coordinate of $i$-th dot.</p>

## Output

<p>Print the sum of results modulo $10^9+7$.</p>





```input1
4
1 2 4 6
```




```input2
5
1 3 5 11 15
```




```output1
11
```




```output2
30
```



## Note

<p>In the first example, for a subset of size $2$, two dots move toward each other, so there is $1$ coordinate where the dots stop.</p><p>For a subset of size $3$, the first dot and third dot move toward the second dot, so there is $1$ coordinate where the dots stop no matter the direction where the second dot moves.</p><p>For $[1, 2, 4, 6]$, the first and second dots move toward each other. For the third dot, initially, the second dot and the fourth dot are the closest dots. Since it is a tie, the third dot moves left. The fourth dot also moves left. So there is $1$ coordinate where the dots stop, which is $1.5$.</p><p>Because there are $6$ subsets of size $2$, $4$ subsets of size $3$ and one subset of size $4$, the answer is $6 \cdot 1 + 4 \cdot 1 + 1 = 11$.</p><p>In the second example, for a subset of size $5$ (when there are dots at $1$, $3$, $5$, $11$, $15$), dots at $1$ and $11$ will move right and dots at $3$, $5$, $15$ will move left. Dots at $1$, $3$, $5$ will eventually meet at $2$, and dots at $11$ and $15$ will meet at $13$, so there are $2$ coordinates where the dots stop.</p>
