## Description

<div><p>Polycarp has $26$ tasks. Each task is designated by a capital letter of the Latin alphabet.</p><p>The teacher asked Polycarp to solve tasks in the following way: if Polycarp began to solve some task, then he must solve it to the end, without being distracted by another task. After switching to another task, Polycarp cannot return to the previous task.</p><p>Polycarp can only solve one task during the day. Every day he wrote down what task he solved. Now the teacher wants to know if Polycarp followed his advice.</p><p>For example, if Polycarp solved tasks in the following order: "<span class="tex-font-style-tt">DDBBCCCBBEZ</span>", then the teacher will see that on the third day Polycarp began to solve the task '<span class="tex-font-style-tt">B</span>', then on the fifth day he got distracted and began to solve the task '<span class="tex-font-style-tt">C</span>', on the eighth day Polycarp returned to the task '<span class="tex-font-style-tt">B</span>'. Other examples of when the teacher is suspicious: "<span class="tex-font-style-tt">BAB</span>", "<span class="tex-font-style-tt">AABBCCDDEEBZZ</span>" and "<span class="tex-font-style-tt">AAAAZAAAAA</span>".</p><p>If Polycarp solved the tasks as follows: "<span class="tex-font-style-tt">FFGZZZY</span>", then the teacher cannot have any suspicions. Please note that Polycarp is not obligated to solve all tasks. Other examples of when the teacher doesn't have any suspicious: "<span class="tex-font-style-tt">BA</span>", "<span class="tex-font-style-tt">AFFFCC</span>" and "<span class="tex-font-style-tt">YYYYY</span>".</p><p>Help Polycarp find out if his teacher might be suspicious.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 1000$). Then $t$ test cases follow.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 50$)&nbsp;— the number of days during which Polycarp solved tasks.</p><p>The second line contains a string of length $n$, consisting of uppercase Latin letters, which is the order in which Polycarp solved the tasks.</p></div><div class="output-specification"><p>For each test case output: </p><ul> <li> "<span class="tex-font-style-tt">YES</span>", if the teacher <span class="tex-font-style-bf">cannot be suspicious</span>; </li><li> "<span class="tex-font-style-tt">NO</span>", otherwise. </li></ul><p>You may print every letter in any case you want (so, for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> are all recognized as positive answer).</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 1000$). Then $t$ test cases follow.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 50$)&nbsp;— the number of days during which Polycarp solved tasks.</p><p>The second line contains a string of length $n$, consisting of uppercase Latin letters, which is the order in which Polycarp solved the tasks.</p>

## Output

<p>For each test case output: </p><ul> <li> "<span class="tex-font-style-tt">YES</span>", if the teacher <span class="tex-font-style-bf">cannot be suspicious</span>; </li><li> "<span class="tex-font-style-tt">NO</span>", otherwise. </li></ul><p>You may print every letter in any case you want (so, for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> are all recognized as positive answer).</p>





```input1
5
3
ABA
11
DDBBCCCBBEZ
7
FFGZZZY
1
Z
2
AB
```




```output1
NO
NO
YES
YES
YES
```


