## Description

<div><p>You have three piles of candies: red, green and blue candies:</p><ul> <li> the first pile contains only red candies and there are $r$ candies in it, </li><li> the second pile contains only green candies and there are $g$ candies in it, </li><li> the third pile contains only blue candies and there are $b$ candies in it. </li></ul><p>Each day Tanya eats exactly two candies of different colors. She is free to choose the colors of eaten candies: the only restriction that she can't eat two candies of the same color in a day.</p><p>Find the maximal number of days Tanya can eat candies? Each day she needs to eat <span class="tex-font-style-bf">exactly</span> two candies.</p></div><div class="input-specification"><p>The first line contains integer $t$ ($1 \le t \le 1000$) — the number of test cases in the input. Then $t$ test cases follow.</p><p>Each test case is given as a separate line of the input. It contains three integers $r$, $g$ and $b$ ($1 \le r, g, b \le 10^8$) — the number of red, green and blue candies, respectively.</p></div><div class="output-specification"><p>Print $t$ integers: the $i$-th printed integer is the answer on the $i$-th test case in the input.</p></div>

## Input

<p>The first line contains integer $t$ ($1 \le t \le 1000$) — the number of test cases in the input. Then $t$ test cases follow.</p><p>Each test case is given as a separate line of the input. It contains three integers $r$, $g$ and $b$ ($1 \le r, g, b \le 10^8$) — the number of red, green and blue candies, respectively.</p>

## Output

<p>Print $t$ integers: the $i$-th printed integer is the answer on the $i$-th test case in the input.</p>





```input1
6
1 1 1
1 2 1
4 1 1
7 4 10
8 1 4
8 2 8
```




```output1
1
2
2
10
5
9
```



## Note

<p>In the first example, Tanya can eat candies for one day only. She can eat any pair of candies this day because all of them have different colors.</p><p>In the second example, Tanya can eat candies for two days. For example, she can eat red and green candies on the first day, and green and blue candies on the second day.</p><p>In the third example, Tanya can eat candies for two days. For example, she can eat red and green candies on the first day, and red and blue candies on the second day. Note, that two red candies will remain uneaten.</p>
