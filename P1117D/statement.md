## Description

<div><p>Reziba has many magic gems. Each magic gem can be split into $M$ normal gems. The amount of space each magic (and normal) gem takes is $1$ unit. A normal gem cannot be split.</p><p>Reziba wants to choose a set of magic gems and split some of them, so the total space occupied by the resulting set of gems is $N$ units. If a magic gem is chosen and split, it takes $M$ units of space (since it is split into $M$ gems); if a magic gem is not split, it takes $1$ unit.</p><p>How many different configurations of the resulting set of gems can Reziba have, such that the total amount of space taken is $N$ units? Print the answer modulo $1000000007$ ($10^9+7$). Two configurations are considered different if the number of magic gems Reziba takes to form them differs, or the indices of gems Reziba has to split differ.</p></div><div class="input-specification"><p>The input contains a single line consisting of $2$ integers $N$ and $M$ ($1 \le N \le 10^{18}$, $2 \le M \le 100$).</p></div><div class="output-specification"><p>Print one integer, the total number of configurations of the resulting set of gems, given that the total amount of space taken is $N$ units. Print the answer modulo $1000000007$ ($10^9+7$).</p></div>

## Input

<p>The input contains a single line consisting of $2$ integers $N$ and $M$ ($1 \le N \le 10^{18}$, $2 \le M \le 100$).</p>

## Output

<p>Print one integer, the total number of configurations of the resulting set of gems, given that the total amount of space taken is $N$ units. Print the answer modulo $1000000007$ ($10^9+7$).</p>





```input1
4 2
```




```input2
3 2
```




```output1
5
```




```output2
3
```



## Note

<p>In the first example each magic gem can split into $2$ normal gems, and we know that the total amount of gems are $4$.</p><p>Let $1$ denote a magic gem, and $0$ denote a normal gem.</p><p>The total configurations you can have is: </p><ul> <li> $1 1 1 1$ (None of the gems split); </li><li> $0 0 1 1$ (First magic gem splits into $2$ normal gems); </li><li> $1 0 0 1$ (Second magic gem splits into $2$ normal gems); </li><li> $1 1 0 0$ (Third magic gem splits into $2$ normal gems); </li><li> $0 0 0 0$ (First and second magic gems split into total $4$ normal gems). </li></ul><p>Hence, answer is $5$.</p>
