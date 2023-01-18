## Description

<div><p>Pavel made a photo of his favourite stars in the sky. His camera takes a photo of all points of the sky that belong to some rectangle with sides parallel to the coordinate axes.</p><p>Strictly speaking, it makes a photo of all points with coordinates $(x, y)$, such that $x_1 \leq x \leq x_2$ and $y_1 \leq y \leq y_2$, where $(x_1, y_1)$ and $(x_2, y_2)$ are coordinates of the left bottom and the right top corners of the rectangle being photographed. The area of this rectangle can be zero.</p><p>After taking the photo, Pavel wrote down coordinates of $n$ of his favourite stars which appeared in the photo. These points are not necessarily distinct, there can be multiple stars in the same point of the sky.</p><p>Pavel has lost his camera recently and wants to buy a similar one. Specifically, he wants to know the dimensions of the photo he took earlier. Unfortunately, the photo is also lost. His notes are also of not much help; numbers are written in random order all over his notepad, so it's impossible to tell which numbers specify coordinates of which points.</p><p>Pavel asked you to help him to determine what are the possible dimensions of the photo according to his notes. As there are multiple possible answers, find the dimensions with the minimal possible area of the rectangle.</p></div><div class="input-specification"><p>The first line of the input contains an only integer $n$ ($1 \leq n \leq 100\,000$), the number of points in Pavel's records.</p><p>The second line contains $2 \cdot n$ integers $a_1$, $a_2$, ..., $a_{2 \cdot n}$ ($1 \leq a_i \leq 10^9$), coordinates, written by Pavel in some order.</p></div><div class="output-specification"><p>Print the only integer, the minimal area of the rectangle which could have contained all points from Pavel's records.</p></div>

## Input

<p>The first line of the input contains an only integer $n$ ($1 \leq n \leq 100\,000$), the number of points in Pavel's records.</p><p>The second line contains $2 \cdot n$ integers $a_1$, $a_2$, ..., $a_{2 \cdot n}$ ($1 \leq a_i \leq 10^9$), coordinates, written by Pavel in some order.</p>

## Output

<p>Print the only integer, the minimal area of the rectangle which could have contained all points from Pavel's records.</p>





```input1
4
4 1 3 2 3 2 1 3

```




```input2
3
5 8 5 5 7 5

```




```output1
1
```




```output2
0
```



## Note

<p>In the first sample stars in Pavel's records can be $(1, 3)$, $(1, 3)$, $(2, 3)$, $(2, 4)$. In this case, the minimal area of the rectangle, which contains all these points is $1$ (rectangle with corners at $(1, 3)$ and $(2, 4)$).</p>
