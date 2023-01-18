## Description

<div><p>There are <span class="tex-span"><i>n</i></span> students at Berland State University. Every student has two skills, each measured as a number: <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> — the programming skill and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> — the sports skill.</p><p>It is announced that an Olympiad in programming and sports will be held soon. That's why Berland State University should choose two teams: one to take part in the programming track and one to take part in the sports track.</p><p>There should be exactly <span class="tex-span"><i>p</i></span> students in the programming team and exactly <span class="tex-span"><i>s</i></span> students in the sports team. A student can't be a member of both teams.</p><p>The university management considers that the strength of the university on the Olympiad is equal to the sum of two values: the programming team strength and the sports team strength. The strength of a team is the sum of skills of its members in the corresponding area, so the strength of the programming team is the sum of all <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and the strength of the sports team is the sum of all <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> over corresponding team members.</p><p>Help Berland State University to compose two teams to maximize the total strength of the university on the Olympiad.</p></div><div class="input-specification"><p>The first line contains three positive integer numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>s</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 3000</span>, <span class="tex-span"><i>p</i> + <i>s</i> ≤ <i>n</i></span>) — the number of students, the size of the programming team and the size of the sports team.</p><p>The second line contains <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 3000</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the programming skill of the <span class="tex-span"><i>i</i></span>-th student.</p><p>The third line contains <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 3000</span>), where <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is the sports skill of the <span class="tex-span"><i>i</i></span>-th student.</p></div><div class="output-specification"><p>In the first line, print the the maximum strength of the university on the Olympiad. In the second line, print <span class="tex-span"><i>p</i></span> numbers — the members of the programming team. In the third line, print <span class="tex-span"><i>s</i></span> numbers — the members of the sports team.</p><p>The students are numbered from 1 to <span class="tex-span"><i>n</i></span> as they are given in the input. All numbers printed in the second and in the third lines should be distinct and can be printed in arbitrary order.</p><p>If there are multiple solutions, print any of them.</p></div>

## Input

<p>The first line contains three positive integer numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>s</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 3000</span>, <span class="tex-span"><i>p</i> + <i>s</i> ≤ <i>n</i></span>) — the number of students, the size of the programming team and the size of the sports team.</p><p>The second line contains <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 3000</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the programming skill of the <span class="tex-span"><i>i</i></span>-th student.</p><p>The third line contains <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 3000</span>), where <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is the sports skill of the <span class="tex-span"><i>i</i></span>-th student.</p>

## Output

<p>In the first line, print the the maximum strength of the university on the Olympiad. In the second line, print <span class="tex-span"><i>p</i></span> numbers — the members of the programming team. In the third line, print <span class="tex-span"><i>s</i></span> numbers — the members of the sports team.</p><p>The students are numbered from 1 to <span class="tex-span"><i>n</i></span> as they are given in the input. All numbers printed in the second and in the third lines should be distinct and can be printed in arbitrary order.</p><p>If there are multiple solutions, print any of them.</p>





```input1
5 2 2
1 3 4 5 2
5 3 2 1 4

```




```input2
4 2 2
10 8 8 3
10 7 9 4

```




```input3
5 3 1
5 2 5 1 7
6 3 1 6 3

```




```output1
18
3 4 
1 5 

```




```output2
31
1 2 
3 4 

```




```output3
23
1 3 5 
4 

```


