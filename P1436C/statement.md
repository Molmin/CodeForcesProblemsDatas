## Description

<div><p>Andrey thinks he is truly a successful developer, but in reality he didn't know about the binary search algorithm until recently. After reading some literature Andrey understood that this algorithm allows to quickly find a certain number $x$ in an array. For an array $a$ indexed from zero, and an integer $x$ the pseudocode of the algorithm is as follows:</p><center> <img class="tex-graphics" src="file://OlX0BvT1.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Note that the elements of the array are indexed from zero, and the division is done in integers (rounding down).</p><p>Andrey read that the algorithm only works if the array is sorted. However, he found this statement untrue, because there certainly exist unsorted arrays for which the algorithm find $x$!</p><p>Andrey wants to write a letter to the book authors, but before doing that he must consider the permutations of size $n$ such that the algorithm finds $x$ in them. A permutation of size $n$ is an array consisting of $n$ distinct integers between $1$ and $n$ in arbitrary order.</p><p>Help Andrey and find the number of permutations of size $n$ which contain $x$ at position $pos$ and for which the given implementation of the binary search algorithm finds $x$ (returns true). As the result may be extremely large, print the remainder of its division by $10^9+7$.</p></div><div class="input-specification"><p>The only line of input contains integers $n$, $x$ and $pos$ ($1 \le x \le n \le 1000$, $0 \le pos \le n - 1$) — the required length of the permutation, the number to search, and the required position of that number, respectively.</p></div><div class="output-specification"><p>Print a single number&nbsp;— the remainder of the division of the number of valid permutations by $10^9+7$.</p></div>

## Input

<p>The only line of input contains integers $n$, $x$ and $pos$ ($1 \le x \le n \le 1000$, $0 \le pos \le n - 1$) — the required length of the permutation, the number to search, and the required position of that number, respectively.</p>

## Output

<p>Print a single number&nbsp;— the remainder of the division of the number of valid permutations by $10^9+7$.</p>





```input1
4 1 2
```




```input2
123 42 24
```




```output1
6
```




```output2
824071958
```



## Note

<p>All possible permutations in the first test case: $(2, 3, 1, 4)$, $(2, 4, 1, 3)$, $(3, 2, 1, 4)$, $(3, 4, 1, 2)$, $(4, 2, 1, 3)$, $(4, 3, 1, 2)$.</p>
