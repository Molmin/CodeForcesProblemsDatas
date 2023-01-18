## Description

<div><p>Polycarp is the project manager in the IT-company. Right now, he needs to choose developers for his team to start a new project. The company has $n$ developers "on the bench" (i.e not involved in other projects). Polycarp assessed the skills of each of them: $a_i$ ($-10^4 \le a_i \le 10^4$) — an integer characteristic of the $i$-th developer. This value can be either positive, zero or even negative (some developers cause distractions).</p><p>After Polycarp chooses a subset of developers for his team, the strength of the team will be determined by the sum of $a_i$ values for all selected developers.</p><p>Polycarp fears that if he chooses a team in such a way that maximizes the sum of the characteristics of $a_i$, other managers may find this unacceptable. For this reason, he plans to create such a team that the sum of the $a_i$ values for it is <span class="tex-font-style-bf">strictly less</span> than the maximum possible value.</p><p>Help Polycarp choose any team that:</p><ul> <li> the sum of the characteristics $a_i$ for all members of the selected team is strictly less than the maximum value that can be achieved by choosing the team in some other way </li><li> and at the same time, the sum of the characteristics of $a_i$ for all members of the selected team is the greatest possible. </li></ul><p>If, following the requirements above, you can select a team in several ways, then just find any of them. </p><p>It's guaranteed that <span class="tex-font-style-bf">the sum of the characteristics in the desired subset is strictly positive</span> (i.e. Polycarp can always choose a non-empty team).</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>Each test case begins with a line containing one integer $n$ ($2 \le n \le 10^5$) — the number of developers "on the bench".</p><p>The second line of a test case contains a sequence of integers $a_1, a_2, \dots, a_n$ ($-10^4 \le a_i \le 10^4$) — the characteristics of the $n$ developers. It is guaranteed that the characteristics are such that <span class="tex-font-style-bf">the sum of the characteristics in the answer is strictly positive</span>.</p><p>It is guaranteed that the sum of $n$ over all test cases in the input doesn't exceed $10^5$.</p></div><div class="output-specification"><p>Print the answers for the given $t$ test cases in the order that they appear in the input. In the first line of each answer, print a positive integer $s$ — the sum of the characteristics in the desired subset. The second line should contain only the characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span> and match the answer:</p><ul> <li> the character in the $i$-th position should be equal to <span class="tex-font-style-tt">1</span> if the $i$-th developer belongs to the team; </li><li> the character in the $i$-th position should be equal to <span class="tex-font-style-tt">0</span> if the $i$-th developer does not belong to the team. </li></ul><p>If there are several answers, print any of them.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>Each test case begins with a line containing one integer $n$ ($2 \le n \le 10^5$) — the number of developers "on the bench".</p><p>The second line of a test case contains a sequence of integers $a_1, a_2, \dots, a_n$ ($-10^4 \le a_i \le 10^4$) — the characteristics of the $n$ developers. It is guaranteed that the characteristics are such that <span class="tex-font-style-bf">the sum of the characteristics in the answer is strictly positive</span>.</p><p>It is guaranteed that the sum of $n$ over all test cases in the input doesn't exceed $10^5$.</p>

## Output

<p>Print the answers for the given $t$ test cases in the order that they appear in the input. In the first line of each answer, print a positive integer $s$ — the sum of the characteristics in the desired subset. The second line should contain only the characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span> and match the answer:</p><ul> <li> the character in the $i$-th position should be equal to <span class="tex-font-style-tt">1</span> if the $i$-th developer belongs to the team; </li><li> the character in the $i$-th position should be equal to <span class="tex-font-style-tt">0</span> if the $i$-th developer does not belong to the team. </li></ul><p>If there are several answers, print any of them.</p>





```input1
5
5
1 -1 1 -1 1
2
11 1
3
5 -3 4
3
5 3 -4
5
-1 0 3 -3 0
```




```output1
2
11101
11
10
6
111
5
100
2
10100
```



## Note

<p>In the first test case, the maximum subset $a_1, a_3, a_5$ has a sum equal to $3$, so Polycarp should choose a team with the maximum total sum which is less than $3$.</p><p>In the second test case, the maximum subset $a_1, a_2$ has a sum equal to $12$, so Polycarp should choose a team with the maximum total sum which is less than $12$.</p><p>In the third test case, the maximum subset $a_1, a_3$ has a sum equal to $9$.</p><p>In the fourth test case, the maximum subset $a_1, a_2$ has a sum equal to $8$.</p><p>In the fifth test case, there are several subsets with a maximum sum equal to $3$, so Polycarp should choose a team with a lower total sum.</p>
