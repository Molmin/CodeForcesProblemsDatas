## Description

<div><p>Sasha is a very happy guy, that's why he is always on the move. There are $n$ cities in the country where Sasha lives. They are all located on one straight line, and for convenience, they are numbered from $1$ to $n$ in increasing order. The distance between any two adjacent cities is equal to $1$ kilometer. Since all roads in the country are directed, it's possible to reach the city $y$ from the city $x$ only if $x &lt; y$. </p><p>Once Sasha decided to go on a trip around the country and to visit all $n$ cities. He will move with the help of his car, <span class="tex-font-style-it">Cheetah-2677</span>. The tank capacity of this model is $v$ liters, and it spends exactly $1$ liter of fuel for $1$ kilometer of the way. At the beginning of the journey, the tank is empty. Sasha is located in the city with the number $1$ and wants to get to the city with the number $n$. There is a gas station in each city. In the $i$-th city, the price of $1$ liter of fuel is $i$ dollars. It is obvious that at any moment of time, the tank can contain at most $v$ liters of fuel.</p><p>Sasha doesn't like to waste money, that's why he wants to know what is the minimum amount of money is needed to finish the trip if he can buy fuel in any city he wants. Help him to figure it out!</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $v$ ($2 \le n \le 100$, $1 \le v \le 100$) &nbsp;— the number of cities in the country and the capacity of the tank.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the minimum amount of money that is needed to finish the trip.</p></div>

## Input

<p>The first line contains two integers $n$ and $v$ ($2 \le n \le 100$, $1 \le v \le 100$) &nbsp;— the number of cities in the country and the capacity of the tank.</p>

## Output

<p>Print one integer&nbsp;— the minimum amount of money that is needed to finish the trip.</p>





```input1
4 2
```




```input2
7 6
```




```output1
4
```




```output2
6
```



## Note

<p>In the first example, Sasha can buy $2$ liters for $2$ dollars ($1$ dollar per liter) in the first city, drive to the second city, spend $1$ liter of fuel on it, then buy $1$ liter for $2$ dollars in the second city and then drive to the $4$-th city. Therefore, the answer is $1+1+2=4$.</p><p>In the second example, the capacity of the tank allows to fill the tank completely in the first city, and drive to the last city without stops in other cities.</p>
