## Description

<div><p>You have received data from a Bubble bot. You know your task is to make factory facilities, but before you even start, you need to know how big the factory is and how many rooms it has. When you look at the data you see that you have the dimensions of the construction, which is in rectangle shape: N x M. </p><p>Then in the next N lines you have M numbers. These numbers represent factory tiles and they can go from 0 to 15. Each of these numbers should be looked in its binary form. Because from each number you know on which side the tile has walls. For example number 10 in it's binary form is 1010, which means that it has a wall from the <span class="tex-font-style-bf">North</span> side, it doesn't have a wall from the <span class="tex-font-style-bf">East</span>, it has a wall on the <span class="tex-font-style-bf">South</span> side and it doesn't have a wall on the <span class="tex-font-style-bf">West</span> side. So it goes North, East, South, West. </p><p>It is guaranteed that the construction always has walls on it's edges. The input will be correct. </p><p>Your task is to print the size of the rooms from biggest to smallest. </p></div><div class="input-specification"><p>The first line has two numbers which are N and M, the size of the construction. Both are integers: </p><p>$n$ ($1 \leq n \leq 10^3$)</p><p>$m$ ($1 \leq m \leq 10^3$)</p><p>Next N x M numbers represent each tile of construction.</p></div><div class="output-specification"><p>Once you finish processing the data your output consists of one line sorted from <span class="tex-font-style-bf">biggest</span> to <span class="tex-font-style-bf">smallest</span> room sizes. </p></div>

## Input

<p>The first line has two numbers which are N and M, the size of the construction. Both are integers: </p><p>$n$ ($1 \leq n \leq 10^3$)</p><p>$m$ ($1 \leq m \leq 10^3$)</p><p>Next N x M numbers represent each tile of construction.</p>

## Output

<p>Once you finish processing the data your output consists of one line sorted from <span class="tex-font-style-bf">biggest</span> to <span class="tex-font-style-bf">smallest</span> room sizes. </p>





```input1
4 5
9 14 11 12 13
5 15 11 6 7
5 9 14 9 14
3 2 14 3 14
```




```output1
9 4 4 2 1
```


