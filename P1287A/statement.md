## Description

<div><p>It's a walking tour day in SIS.Winter, so $t$ groups of students are visiting Torzhok. Streets of Torzhok are so narrow that students have to go in a row one after another.</p><p>Initially, some students are angry. Let's describe a group of students by a string of capital letters "<span class="tex-font-style-tt">A</span>" and "<span class="tex-font-style-tt">P</span>": </p><ul> <li> "<span class="tex-font-style-tt">A</span>" corresponds to an angry student </li><li> "<span class="tex-font-style-tt">P</span>" corresponds to a patient student </li></ul><p>Such string describes the row from the last to the first student.</p><p>Every minute every angry student throws a snowball at the next student. Formally, if an angry student corresponds to the character with index $i$ in the string describing a group then they will throw a snowball at the student that corresponds to the character with index $i+1$ (students are given from the last to the first student). If the target student was not angry yet, they become angry. Even if the first (the rightmost in the string) student is angry, they don't throw a snowball since there is no one in front of them.</p><center><img class="tex-graphics" src="file://g7Vf8ntL.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>Let's look at the first example test. The row initially looks like this: <span class="tex-font-style-tt">PPAP</span>. Then, after a minute the only single angry student will throw a snowball at the student in front of them, and they also become angry: <span class="tex-font-style-tt">PPAA</span>. After that, no more students will become angry.</p><p>Your task is to help SIS.Winter teachers to determine the last moment a student becomes angry for every group.</p></div><div class="input-specification"><p>The first line contains a single integer $t$&nbsp;— the number of groups of students ($1 \le t \le 100$). The following $2t$ lines contain descriptions of groups of students.</p><p>The description of the group starts with an integer $k_i$ ($1 \le k_i \le 100$)&nbsp;— the number of students in the group, followed by a string $s_i$, consisting of $k_i$ letters "<span class="tex-font-style-tt">A</span>" and "<span class="tex-font-style-tt">P</span>", which describes the $i$-th group of students.</p></div><div class="output-specification"><p>For every group output single integer&nbsp;— the last moment a student becomes angry.</p></div>

## Input

<p>The first line contains a single integer $t$&nbsp;— the number of groups of students ($1 \le t \le 100$). The following $2t$ lines contain descriptions of groups of students.</p><p>The description of the group starts with an integer $k_i$ ($1 \le k_i \le 100$)&nbsp;— the number of students in the group, followed by a string $s_i$, consisting of $k_i$ letters "<span class="tex-font-style-tt">A</span>" and "<span class="tex-font-style-tt">P</span>", which describes the $i$-th group of students.</p>

## Output

<p>For every group output single integer&nbsp;— the last moment a student becomes angry.</p>





```input1
1
4
PPAP
```




```input2
3
12
APPAPPPAPPPP
3
AAP
3
PPA
```




```output1
1
```




```output2
4
1
0
```



## Note

<p>In the first test, after $1$ minute the state of students becomes <span class="tex-font-style-tt">PPAA</span>. After that, no new angry students will appear.</p><p>In the second tets, state of students in the first group is: </p><ul> <li> after $1$ minute&nbsp;— <span class="tex-font-style-tt">AAPAAPPAAPPP</span> </li><li> after $2$ minutes&nbsp;— <span class="tex-font-style-tt">AAAAAAPAAAPP</span> </li><li> after $3$ minutes&nbsp;— <span class="tex-font-style-tt">AAAAAAAAAAAP</span> </li><li> after $4$ minutes all $12$ students are angry </li></ul><p>In the second group after $1$ minute, all students are angry.</p>
