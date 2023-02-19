## Description

<div><p>Alice and Bob received $n$ candies from their parents. <span class="tex-font-style-bf">Each candy weighs either 1 gram or 2 grams</span>. Now they want to divide all candies among themselves fairly so that the total weight of Alice's candies is equal to the total weight of Bob's candies.</p><p>Check if they can do that.</p><p>Note that candies <span class="tex-font-style-bf">are not allowed to be cut in half</span>.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. Then $t$ test cases follow.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 100$)&nbsp;— the number of candies that Alice and Bob received.</p><p>The next line contains $n$ integers $a_1, a_2, \ldots, a_n$&nbsp;— the weights of the candies. The weight of each candy is either $1$ or $2$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, output on a separate line: </p><ul> <li> "<span class="tex-font-style-tt">YES</span>", if all candies can be divided into two sets with the same weight; </li><li> "<span class="tex-font-style-tt">NO</span>" otherwise. </li></ul><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will be recognized as positive).</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. Then $t$ test cases follow.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 100$)&nbsp;— the number of candies that Alice and Bob received.</p><p>The next line contains $n$ integers $a_1, a_2, \ldots, a_n$&nbsp;— the weights of the candies. The weight of each candy is either $1$ or $2$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, output on a separate line: </p><ul> <li> "<span class="tex-font-style-tt">YES</span>", if all candies can be divided into two sets with the same weight; </li><li> "<span class="tex-font-style-tt">NO</span>" otherwise. </li></ul><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will be recognized as positive).</p>





```input1
5
2
1 1
2
1 2
4
1 2 1 2
3
2 2 2
3
2 1 2
```




```output1
YES
NO
YES
NO
NO
```



## Note

<p>In the first test case, Alice and Bob can each take one candy, then both will have a total weight of $1$.</p><p>In the second test case, any division will be unfair.</p><p>In the third test case, both Alice and Bob can take two candies, one of weight $1$ and one of weight $2$.</p><p>In the fourth test case, it is impossible to divide three identical candies between two people.</p><p>In the fifth test case, any division will also be unfair.</p>
