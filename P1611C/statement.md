## Description

<div><p>Polycarp wrote on a whiteboard an array $p$ of length $n$, which is a permutation of numbers from $1$ to $n$. In other words, in $p$ each number from $1$ to $n$ occurs exactly once.</p><p>He also prepared a resulting array $a$, which is initially empty (that is, it has a length of $0$).</p><p>After that, he did exactly $n$ <span class="tex-font-style-it">steps</span>. Each <span class="tex-font-style-it">step</span> looked like this:</p><ul> <li> Look at the leftmost and rightmost elements of $p$, and pick the smaller of the two.</li><li> If you picked the leftmost element of $p$, append it to the left of $a$; otherwise, if you picked the rightmost element of $p$, append it to the right of $a$.</li><li> The picked element is erased from $p$. </li></ul><p>Note that on the last step, $p$ has a length of $1$ and its minimum element is both leftmost and rightmost. In this case, Polycarp can choose what role the minimum element plays. In other words, this element can be added to $a$ both on the left and on the right (at the discretion of Polycarp).</p><p>Let's look at an example. Let $n=4$, $p=[3, 1, 4, 2]$. Initially $a=[]$. Then:</p><ul><li> During the first step, the minimum is on the right (with a value of $2$), so after this step, $p=[3,1,4]$ and $a=[2]$ (he added the value $2$ to the right). </li><li> During the second step, the minimum is on the left (with a value of $3$), so after this step, $p=[1,4]$ and $a=[3,2]$ (he added the value $3$ to the left). </li><li> During the third step, the minimum is on the left (with a value of $1$), so after this step, $p=[4]$ and $a=[1,3,2]$ (he added the value $1$ to the left). </li><li> During the fourth step, the minimum is both left and right (this value is $4$). Let's say Polycarp chose the right option. After this step, $p=[]$ and $a=[1,3,2,4]$ (he added the value $4$ to the right).</li></ul><p>Thus, a possible value of $a$ after $n$ steps could be $a=[1,3,2,4]$.</p><p>You are given the final value of the resulting array $a$. Find <span class="tex-font-style-bf">any</span> possible initial value for $p$ that can result the given $a$, or determine that there is no solution.</p></div><div class="input-specification"><p>The first line of the input contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases in the test.</p><p>Each test case consists of two lines. The first of them contains an integer $n$ ($1 \le n \le 2\cdot10^5$) — the length of the array $a$. The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$) — the elements of the array $a$. All elements of the $a$ array are distinct numbers.</p><p>It is guaranteed that the sum of the values $n$ over all test cases in the test does not exceed $2\cdot10^5$.</p></div><div class="output-specification"><p>Print $t$ lines, each of the lines must contain the answer to the corresponding set of input data: numbers $p_1, p_2, \dots, p_n$ &nbsp;— any of the possible initial values of the array $p$, which will lead to the given array $a$. All elements of $p$ are distinct integers from $1$ to $n$. Thus, if there are several solutions, print any. If there is no solution, then print <span class="tex-font-style-tt">-1</span> on the line.</p></div>

## Input

<p>The first line of the input contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases in the test.</p><p>Each test case consists of two lines. The first of them contains an integer $n$ ($1 \le n \le 2\cdot10^5$) — the length of the array $a$. The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$) — the elements of the array $a$. All elements of the $a$ array are distinct numbers.</p><p>It is guaranteed that the sum of the values $n$ over all test cases in the test does not exceed $2\cdot10^5$.</p>

## Output

<p>Print $t$ lines, each of the lines must contain the answer to the corresponding set of input data: numbers $p_1, p_2, \dots, p_n$ &nbsp;— any of the possible initial values of the array $p$, which will lead to the given array $a$. All elements of $p$ are distinct integers from $1$ to $n$. Thus, if there are several solutions, print any. If there is no solution, then print <span class="tex-font-style-tt">-1</span> on the line.</p>





```input1
4
4
1 3 2 4
1
1
5
1 3 5 4 2
3
3 2 1
```




```output1
3 1 4 2
1
-1
2 3 1
```



## Note

<p>The first test case in the example is clarified in the main section of the problem statement. There may be other correct answers for this test set.</p><p>In the second test case, $n=1$. Thus, there is only one permutation that can be the answer: $p=[1]$. Indeed, this is the answer to this test case.</p><p>In the third test case of the example, no matter what permutation you take as $p$, after applying the $n$ steps, the result will differ from $a=[1, 3, 5, 4, 2]$.</p>
