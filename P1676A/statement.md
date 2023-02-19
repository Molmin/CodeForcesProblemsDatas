## Description

<div><p>A ticket is a string consisting of six digits. A ticket is considered lucky if the sum of the first three digits is equal to the sum of the last three digits. Given a ticket, output if it is lucky or not. Note that a ticket can have leading zeroes.</p></div><div class="input-specification"><p>The first line of the input contains an integer $t$ ($1 \leq t \leq 10^3$)&nbsp;— the number of testcases.</p><p>The description of each test consists of one line containing one string consisting of six digits.</p></div><div class="output-specification"><p>Output $t$ lines, each of which contains the answer to the corresponding test case. Output "<span class="tex-font-style-tt">YES</span>" if the given ticket is lucky, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can output the answer in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p></div>

## Input

<p>The first line of the input contains an integer $t$ ($1 \leq t \leq 10^3$)&nbsp;— the number of testcases.</p><p>The description of each test consists of one line containing one string consisting of six digits.</p>

## Output

<p>Output $t$ lines, each of which contains the answer to the corresponding test case. Output "<span class="tex-font-style-tt">YES</span>" if the given ticket is lucky, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can output the answer in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p>





```input1
5
213132
973894
045207
000000
055776
```




```output1
YES
NO
YES
YES
NO
```



## Note

<p>In the first test case, the sum of the first three digits is $2 + 1 + 3 = 6$ and the sum of the last three digits is $1 + 3 + 2 = 6$, they are equal so the answer is "<span class="tex-font-style-tt">YES</span>".</p><p>In the second test case, the sum of the first three digits is $9 + 7 + 3 = 19$ and the sum of the last three digits is $8 + 9 + 4 = 21$, they are not equal so the answer is "<span class="tex-font-style-tt">NO</span>".</p><p>In the third test case, the sum of the first three digits is $0 + 4 + 5 = 9$ and the sum of the last three digits is $2 + 0 + 7 = 9$, they are equal so the answer is "<span class="tex-font-style-tt">YES</span>".</p>
