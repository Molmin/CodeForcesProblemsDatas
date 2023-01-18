## Description

<div><p>A positive integer is called <span class="tex-font-style-it">composite</span> if it can be represented as a product of two positive integers, both greater than $1$. For example, the following numbers are composite: $6$, $4$, $120$, $27$. The following numbers aren't: $1$, $2$, $3$, $17$, $97$.</p><p>Alice is given a sequence of $n$ composite numbers $a_1,a_2,\ldots,a_n$.</p><p>She wants to choose an integer $m \le 11$ and color each element one of $m$ colors from $1$ to $m$ so that:</p><ul> <li> for each color from $1$ to $m$ there is at least one element of this color; </li><li> each element is colored and colored exactly one color; </li><li> the greatest common divisor of any two elements that are colored the same color is greater than $1$, i.e. $\gcd(a_i, a_j)&gt;1$ for each pair $i, j$ if these elements are colored the same color. </li></ul><p>Note that equal elements can be colored different colors&nbsp;— you just have to choose one of $m$ colors for each of the indices from $1$ to $n$.</p><p>Alice showed already that if all $a_i \le 1000$ then she can always solve the task by choosing some $m \le 11$.</p><p>Help Alice to find the required coloring. Note that you don't have to minimize or maximize the number of colors, you just have to find the solution with some $m$ from $1$ to $11$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$) — the number of test cases. Then the descriptions of the test cases follow.</p><p>The first line of the test case contains a single integer $n$ ($1 \le n \le 1000$) — the amount of numbers in a sequence $a$.</p><p>The second line of the test case contains $n$ composite integers $a_1,a_2,\ldots,a_n$ ($4 \le a_i \le 1000$).</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $10^4$.</p></div><div class="output-specification"><p>For each test case print $2$ lines. The first line should contain a single integer $m$ ($1 \le m \le 11$) — the number of used colors. Consider colors to be numbered from $1$ to $m$. The second line should contain any coloring that satisfies the above conditions. Print $n$ integers $c_1, c_2, \dots, c_n$ ($1 \le c_i \le m$), where $c_i$ is the color of the $i$-th element. If there are multiple solutions then you can print any of them. Note that you don't have to minimize or maximize the number of colors, you just have to find the solution with some $m$ from $1$ to $11$.</p><p>Remember that each color from $1$ to $m$ should be used at least once. Any two elements of the same color should not be coprime (i.e. their GCD should be greater than $1$).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$) — the number of test cases. Then the descriptions of the test cases follow.</p><p>The first line of the test case contains a single integer $n$ ($1 \le n \le 1000$) — the amount of numbers in a sequence $a$.</p><p>The second line of the test case contains $n$ composite integers $a_1,a_2,\ldots,a_n$ ($4 \le a_i \le 1000$).</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $10^4$.</p>

## Output

<p>For each test case print $2$ lines. The first line should contain a single integer $m$ ($1 \le m \le 11$) — the number of used colors. Consider colors to be numbered from $1$ to $m$. The second line should contain any coloring that satisfies the above conditions. Print $n$ integers $c_1, c_2, \dots, c_n$ ($1 \le c_i \le m$), where $c_i$ is the color of the $i$-th element. If there are multiple solutions then you can print any of them. Note that you don't have to minimize or maximize the number of colors, you just have to find the solution with some $m$ from $1$ to $11$.</p><p>Remember that each color from $1$ to $m$ should be used at least once. Any two elements of the same color should not be coprime (i.e. their GCD should be greater than $1$).</p>





```input1
3
3
6 10 15
2
4 9
23
437 519 865 808 909 391 194 291 237 395 323 365 511 497 781 737 871 559 731 697 779 841 961
```




```output1
1
1 1 1
2
2 1
11
4 7 8 10 7 3 10 7 7 8 3 1 1 5 5 9 2 2 3 3 4 11 6
```



## Note

<p>In the first test case, $\gcd(6,10)=2$, $\gcd(6,15)=3$ and $\gcd(10,15)=5$. Therefore, it's valid to color all elements the same color. Note that there are other colorings which satisfy Alice's requirement in this test case.</p><p>In the second test case there is only one element of each color, so the coloring definitely satisfies Alice's requirement.</p>
