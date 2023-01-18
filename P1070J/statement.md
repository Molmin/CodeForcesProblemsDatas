## Description

<div><p>Berhattan is the capital of Berland. There are $n$ streets running parallel in the east-west direction (horizontally), and there are $m$ avenues running parallel in the south-north direction (vertically). Each street intersects with each avenue, forming a crossroad. So in total there are $n \cdot m$ crossroads in Berhattan.</p><p>Recently, the government has changed in Berland. The new government wants to name all avenues and all streets after heroes of revolution.</p><p>The special committee prepared the list of $k$ names. Only these names can be used as new names for streets and avenues. Each name can be used at most once.</p><p>The members of committee want to name streets and avenues in the way that minimizes inconvenience for residents. They believe that if street and avenue names start with the same letter, then their crossroad will be <span class="tex-font-style-it">inconvenient</span>. Hence only the first letter of each name matters.</p><p>Given first letters of $k$ names, find $C$ — minimal possible number of inconvenient crossroads in Berhattan after the naming process.</p></div><div class="input-specification"><p>Input contains one or several test cases to process. The first line contains $t$ ($1 \le t \le 30000$) — the number of test cases. Solve test cases separately, test cases are completely independent and do not affect each other.</p><p>The description of $t$ test cases follows. Each test case starts with line with space-separated numbers $n, m, k$ ($1 \le n,m \le 30000$; $n+m \le k \le 2\cdot10^5$) — the number of streets, number of avenues and the number of names in the committee's list, respectively.</p><p>The the second line of each test case contains a string of $k$ uppercase English letters. $i$-th letter of the string is the first letter of $i$-th name from the committee's list. </p><p>It's guaranteed that the sum of numbers $n$ from all test cases is not greater than $30000$. Similarly, the sum of numbers $m$ from all test cases is not greater than $30000$. The sum of numbers $k$ from all test cases is not greater than $2\cdot10^5$.</p></div><div class="output-specification"><p>For each test case print single number $C$ in the separate line — minimal possible number of inconvenient crossroads in Berhattan after the naming process.</p></div>

## Input

<p>Input contains one or several test cases to process. The first line contains $t$ ($1 \le t \le 30000$) — the number of test cases. Solve test cases separately, test cases are completely independent and do not affect each other.</p><p>The description of $t$ test cases follows. Each test case starts with line with space-separated numbers $n, m, k$ ($1 \le n,m \le 30000$; $n+m \le k \le 2\cdot10^5$) — the number of streets, number of avenues and the number of names in the committee's list, respectively.</p><p>The the second line of each test case contains a string of $k$ uppercase English letters. $i$-th letter of the string is the first letter of $i$-th name from the committee's list. </p><p>It's guaranteed that the sum of numbers $n$ from all test cases is not greater than $30000$. Similarly, the sum of numbers $m$ from all test cases is not greater than $30000$. The sum of numbers $k$ from all test cases is not greater than $2\cdot10^5$.</p>

## Output

<p>For each test case print single number $C$ in the separate line — minimal possible number of inconvenient crossroads in Berhattan after the naming process.</p>





```input1
2
2 3 9
EEZZEEZZZ
2 7 9
EEZZEEZZZ

```




```input2
2
4 4 8
CZBBCZBC
1 1 4
TTCT

```




```output1
0
4

```




```output2
1
0

```


