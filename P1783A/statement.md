## Description

<div><p>An array $a$ is called <span class="tex-font-style-it">ugly</span> if it contains <span class="tex-font-style-bf">at least one</span> element which is equal to the <span class="tex-font-style-bf">sum of all elements before it</span>. If the array is not ugly, it is <span class="tex-font-style-it">beautiful</span>.</p><p>For example:</p><ul> <li> the array $[6, 3, 9, 6]$ is ugly: the element $9$ is equal to $6 + 3$; </li><li> the array $[5, 5, 7]$ is ugly: the element $5$ (the second one) is equal to $5$; </li><li> the array $[8, 4, 10, 14]$ is beautiful: $8 \ne 0$, $4 \ne 8$, $10 \ne 8 + 4$, $14 \ne 8 + 4 + 10$, so there is no element which is equal to the sum of all elements before it. </li></ul><p>You are given an array $a$ such that $1 \le a_1 \le a_2 \le \dots \le a_n \le 100$. You have to <span class="tex-font-style-bf">reorder</span> the elements of $a$ in such a way that the resulting array is beautiful. Note that you are not allowed to insert new elements or erase existing ones, you can only change the order of elements of $a$. You are allowed to keep the array $a$ unchanged, if it is beautiful.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 2000$) — the number of test cases.</p><p>Each test case consists of two lines. The first line contains one integer $n$ ($2 \le n \le 50$). The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_1 \le a_2 \le \dots \le a_n \le 100$).</p></div><div class="output-specification"><p>For each test case, print the answer as follows:</p><ul> <li> if it is impossible to reorder the elements of $a$ in such a way that it becomes beautiful, print <span class="tex-font-style-tt">NO</span>; </li><li> otherwise, in the first line, print <span class="tex-font-style-tt">YES</span>. In the second line, print $n$ integers — any beautiful array which can be obtained from $a$ by reordering its elements. If there are multiple such arrays, print any of them. </li></ul></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 2000$) — the number of test cases.</p><p>Each test case consists of two lines. The first line contains one integer $n$ ($2 \le n \le 50$). The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_1 \le a_2 \le \dots \le a_n \le 100$).</p>

## Output

<p>For each test case, print the answer as follows:</p><ul> <li> if it is impossible to reorder the elements of $a$ in such a way that it becomes beautiful, print <span class="tex-font-style-tt">NO</span>; </li><li> otherwise, in the first line, print <span class="tex-font-style-tt">YES</span>. In the second line, print $n$ integers — any beautiful array which can be obtained from $a$ by reordering its elements. If there are multiple such arrays, print any of them. </li></ul>





```input1|2,3,6,7
4
4
3 3 6 6
2
10 10
5
1 2 3 4 5
3
1 4 4
```




```output1
YES
3 6 3 6
NO
YES
2 4 1 5 3
YES
1 4 4
```


