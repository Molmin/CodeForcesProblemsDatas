## Description

<div><p>Let's define a number <span class="tex-font-style-it">ebne (even but not even)</span> if and only if its sum of digits is divisible by $2$ but the number itself is not divisible by $2$. For example, $13$, $1227$, $185217$ are <span class="tex-font-style-it">ebne</span> numbers, while $12$, $2$, $177013$, $265918$ are not. If you're still unsure what <span class="tex-font-style-it">ebne</span> numbers are, you can look at the sample notes for more clarification.</p><p>You are given a non-negative integer $s$, consisting of $n$ digits. You can delete some digits (they are <span class="tex-font-style-bf">not</span> necessary consecutive/successive) to make the given number <span class="tex-font-style-it">ebne</span>. You cannot change the order of the digits, that is, after deleting the digits the remaining digits collapse. The resulting number shouldn't contain leading zeros. You can delete any number of digits between $0$ (do not delete any digits at all) and $n-1$.</p><p>For example, if you are given $s=$<span class="tex-font-style-tt">222373204424185217171912</span> then one of possible ways to make it <span class="tex-font-style-it">ebne</span> is: <span class="tex-font-style-tt"><span class="tex-font-style-bf"><span class="tex-font-style-striked">2</span></span>22373<span class="tex-font-style-bf"><span class="tex-font-style-striked">20</span></span>442<span class="tex-font-style-bf"><span class="tex-font-style-striked">4</span></span>18521717191<span class="tex-font-style-bf"><span class="tex-font-style-striked">2</span></span></span> $\rightarrow$ <span class="tex-font-style-tt">2237344218521717191</span>. The sum of digits of <span class="tex-font-style-tt">2237344218521717191</span> is equal to $70$ and is divisible by $2$, but number itself is not divisible by $2$: it means that the resulting number is <span class="tex-font-style-it">ebne</span>.</p><p>Find <span class="tex-font-style-bf">any</span> resulting number that is <span class="tex-font-style-it">ebne</span>. If it's impossible to create an <span class="tex-font-style-it">ebne</span> number from the given number report about it.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 1000$) &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 3000$) &nbsp;— the number of digits in the original number.</p><p>The second line of each test case contains a non-negative integer number $s$, consisting of $n$ digits.</p><p>It is guaranteed that $s$ does not contain leading zeros and the sum of $n$ over all test cases does not exceed $3000$.</p></div><div class="output-specification"><p>For each test case given in the input print the answer in the following format:</p><ul><li> If it is impossible to create an <span class="tex-font-style-it">ebne</span> number, print "<span class="tex-font-style-tt">-1</span>" (without quotes);</li><li> Otherwise, print the resulting number after deleting some, possibly zero, but not all digits. This number should be <span class="tex-font-style-it">ebne</span>. If there are multiple answers, you can print <span class="tex-font-style-bf">any</span> of them. Note that answers with leading zeros or empty strings are not accepted. <span class="tex-font-style-bf">It's not necessary to minimize or maximize the number of deleted digits</span>.</li></ul></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 1000$) &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 3000$) &nbsp;— the number of digits in the original number.</p><p>The second line of each test case contains a non-negative integer number $s$, consisting of $n$ digits.</p><p>It is guaranteed that $s$ does not contain leading zeros and the sum of $n$ over all test cases does not exceed $3000$.</p>

## Output

<p>For each test case given in the input print the answer in the following format:</p><ul><li> If it is impossible to create an <span class="tex-font-style-it">ebne</span> number, print "<span class="tex-font-style-tt">-1</span>" (without quotes);</li><li> Otherwise, print the resulting number after deleting some, possibly zero, but not all digits. This number should be <span class="tex-font-style-it">ebne</span>. If there are multiple answers, you can print <span class="tex-font-style-bf">any</span> of them. Note that answers with leading zeros or empty strings are not accepted. <span class="tex-font-style-bf">It's not necessary to minimize or maximize the number of deleted digits</span>.</li></ul>





```input1
4
4
1227
1
0
6
177013
24
222373204424185217171912
```




```output1
1227
-1
17703
2237344218521717191
```



## Note

<p>In the first test case of the example, $1227$ is already an <span class="tex-font-style-it">ebne</span> number (as $1 + 2 + 2 + 7 = 12$, $12$ is divisible by $2$, while in the same time, $1227$ is not divisible by $2$) so we don't need to delete any digits. Answers such as $127$ and $17$ will also be accepted.</p><p>In the second test case of the example, it is clearly impossible to create an <span class="tex-font-style-it">ebne</span> number from the given number.</p><p>In the third test case of the example, there are many <span class="tex-font-style-it">ebne</span> numbers we can obtain by deleting, for example, $1$ digit such as $17703$, $77013$ or $17013$. Answers such as $1701$ or $770$ will not be accepted as they are not <span class="tex-font-style-it">ebne</span> numbers. Answer $013$ will not be accepted as it contains leading zeroes.</p><p>Explanation:</p><ul><li> $1 + 7 + 7 + 0 + 3 = 18$. As $18$ is divisible by $2$ while $17703$ is not divisible by $2$, we can see that $17703$ is an <span class="tex-font-style-it">ebne</span> number. Same with $77013$ and $17013$;</li><li> $1 + 7 + 0 + 1 = 9$. Because $9$ is not divisible by $2$, $1701$ is not an <span class="tex-font-style-it">ebne</span> number;</li><li> $7 + 7 + 0 = 14$. This time, $14$ is divisible by $2$ but $770$ is also divisible by $2$, therefore, $770$ is not an <span class="tex-font-style-it">ebne</span> number.</li></ul><p>In the last test case of the example, one of many other possible answers is given. Another possible answer is: <span class="tex-font-style-tt">222373204424185217171912</span> $\rightarrow$ <span class="tex-font-style-tt">22237320442418521717191</span> (delete the last digit).</p>
