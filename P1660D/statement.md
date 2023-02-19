## Description

<div><p>You are given an array $a$ consisting of $n$ integers. For each $i$ ($1 \le i \le n$) the following inequality is true: $-2 \le a_i \le 2$.</p><p>You can remove any number (possibly $0$) of elements from the beginning of the array and any number (possibly $0$) of elements from the end of the array. You are allowed to delete the whole array.</p><p>You need to answer the question: how many elements should be removed from the beginning of the array, and how many elements should be removed from the end of the array, so that the result will be an array whose product (multiplication) of elements is <span class="tex-font-style-bf">maximal</span>. If there is more than one way to get an array with the maximum product of elements on it, you are allowed to output <span class="tex-font-style-bf">any</span> of them. </p><p>The product of elements of an <span class="tex-font-style-bf">empty</span> array (array of length $0$) should be assumed to be $1$.</p></div><div class="input-specification"><p>The first line of input data contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;—the number of test cases in the test.</p><p>Then the descriptions of the input test cases follow.</p><p>The first line of each test case description contains an integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;—the length of array $a$.</p><p>The next line contains $n$ integers $a_1, a_2, \dots, a_n$ ($|a_i| \le 2$)&nbsp;— elements of array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output two non-negative numbers $x$ and $y$ ($0 \le x + y \le n$)&nbsp;— such that the product (multiplication) of the array numbers, after removing $x$ elements from the beginning and $y$ elements from the end, is maximal.</p><p>If there is more than one way to get the maximal product, it is allowed to output <span class="tex-font-style-bf">any</span> of them. Consider the product of numbers on <span class="tex-font-style-bf">empty</span> array to be $1$.</p></div>

## Input

<p>The first line of input data contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;—the number of test cases in the test.</p><p>Then the descriptions of the input test cases follow.</p><p>The first line of each test case description contains an integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;—the length of array $a$.</p><p>The next line contains $n$ integers $a_1, a_2, \dots, a_n$ ($|a_i| \le 2$)&nbsp;— elements of array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output two non-negative numbers $x$ and $y$ ($0 \le x + y \le n$)&nbsp;— such that the product (multiplication) of the array numbers, after removing $x$ elements from the beginning and $y$ elements from the end, is maximal.</p><p>If there is more than one way to get the maximal product, it is allowed to output <span class="tex-font-style-bf">any</span> of them. Consider the product of numbers on <span class="tex-font-style-bf">empty</span> array to be $1$.</p>





```input1
5
4
1 2 -1 2
3
1 1 -2
5
2 0 -2 2 -1
3
-2 -1 -1
3
-1 -2 -2
```




```output1
0 2
3 0
2 0
0 1
1 0
```



## Note

<p>In the first case, the maximal value of the product is $2$. Thus, we can either delete the first three elements (obtain array $[2]$), or the last two and one first element (also obtain array $[2]$), or the last two elements (obtain array $[1, 2]$). Thus, in the first case, the answers fit: "<span class="tex-font-style-tt">3 0</span>", or "<span class="tex-font-style-tt">1 2</span>", or "<span class="tex-font-style-tt">0 2</span>".</p><p>In the second case, the maximum value of the product is $1$. Then we can remove all elements from the array because the value of the product on the empty array will be $1$. So the answer is "<span class="tex-font-style-tt">3 0</span>", but there are other possible answers.</p><p>In the third case, we can remove the first two elements of the array. Then we get the array: $[-2, 2, -1]$. The product of the elements of the resulting array is $(-2) \cdot 2 \cdot (-1) = 4$. This value is the maximum possible value that can be obtained. Thus, for this case the answer is: "<span class="tex-font-style-tt">2 0</span>".</p>
