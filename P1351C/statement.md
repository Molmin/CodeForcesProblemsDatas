## Description

<div><p>Skier rides on a snowy field. Its movements can be described by a string of characters '<span class="tex-font-style-tt">S</span>', '<span class="tex-font-style-tt">N</span>', '<span class="tex-font-style-tt">W</span>', '<span class="tex-font-style-tt">E</span>' (which correspond to $1$ meter movement in the south, north, west or east direction respectively).</p><p>It is known that if he moves along a previously unvisited segment of a path (i.e. this segment of the path is visited the first time), then the time of such movement is $5$ seconds. If he rolls along previously visited segment of a path (i.e., this segment of the path has been covered by his path before), then it takes $1$ second.</p><p>Find the skier's time to roll all the path.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases in the input. Then $t$ test cases follow.</p><p>Each set is given by one nonempty string of the characters '<span class="tex-font-style-tt">S</span>', '<span class="tex-font-style-tt">N</span>', '<span class="tex-font-style-tt">W</span>', '<span class="tex-font-style-tt">E</span>'. The length of the string does not exceed $10^5$ characters.</p><p>The sum of the lengths of $t$ given lines over all test cases in the input does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, print the desired path time in seconds.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases in the input. Then $t$ test cases follow.</p><p>Each set is given by one nonempty string of the characters '<span class="tex-font-style-tt">S</span>', '<span class="tex-font-style-tt">N</span>', '<span class="tex-font-style-tt">W</span>', '<span class="tex-font-style-tt">E</span>'. The length of the string does not exceed $10^5$ characters.</p><p>The sum of the lengths of $t$ given lines over all test cases in the input does not exceed $10^5$.</p>

## Output

<p>For each test case, print the desired path time in seconds.</p>





```input1
5
NNN
NS
WWEN
WWEE
NWNWS
```




```output1
15
6
16
12
25
```


