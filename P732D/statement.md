## Description

<div><p>Vasiliy has an exam period which will continue for <span class="tex-span"><i>n</i></span> days. He has to pass exams on <span class="tex-span"><i>m</i></span> subjects. Subjects are numbered from 1 to <span class="tex-span"><i>m</i></span>.</p><p>About every day we know exam for which one of <span class="tex-span"><i>m</i></span> subjects can be passed on that day. Perhaps, some day you can't pass any exam. It is not allowed to pass more than one exam on any day. </p><p>On each day Vasiliy can either pass the exam of that day (it takes the whole day) or prepare all day for some exam or have a rest. </p><p>About each subject Vasiliy know a number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— the number of days he should prepare to pass the exam number <span class="tex-span"><i>i</i></span>. Vasiliy can switch subjects while preparing for exams, it is not necessary to prepare continuously during <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> days for the exam number <span class="tex-span"><i>i</i></span>. He can mix the order of preparation for exams in any way.</p><p>Your task is to determine the minimum number of days in which Vasiliy can pass all exams, or determine that it is impossible. Each exam should be passed exactly one time. </p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of days in the exam period and the number of subjects. </p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>d</i><sub class="lower-index">1</sub>, <i>d</i><sub class="lower-index">2</sub>, ..., <i>d</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>), where <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> is the number of subject, the exam of which can be passed on the day number <span class="tex-span"><i>i</i></span>. If <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> equals 0, it is not allowed to pass any exams on the day number <span class="tex-span"><i>i</i></span>. </p><p>The third line contains <span class="tex-span"><i>m</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of days that are needed to prepare before passing the exam on the subject <span class="tex-span"><i>i</i></span>.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the minimum number of days in which Vasiliy can pass all exams. If it is impossible, print <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of days in the exam period and the number of subjects. </p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>d</i><sub class="lower-index">1</sub>, <i>d</i><sub class="lower-index">2</sub>, ..., <i>d</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>), where <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> is the number of subject, the exam of which can be passed on the day number <span class="tex-span"><i>i</i></span>. If <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> equals 0, it is not allowed to pass any exams on the day number <span class="tex-span"><i>i</i></span>. </p><p>The third line contains <span class="tex-span"><i>m</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of days that are needed to prepare before passing the exam on the subject <span class="tex-span"><i>i</i></span>.</p>

## Output

<p>Print one integer&nbsp;— the minimum number of days in which Vasiliy can pass all exams. If it is impossible, print <span class="tex-font-style-tt">-1</span>.</p>





```input1
7 2
0 1 0 2 1 0 2
2 1

```




```input2
10 3
0 0 1 2 3 0 2 0 1 2
1 1 4

```




```input3
5 1
1 1 1 1 1
5

```




```output1
5

```




```output2
9

```




```output3
-1

```



## Note

<p>In the first example Vasiliy can behave as follows. On the first and the second day he can prepare for the exam number 1 and pass it on the fifth day, prepare for the exam number 2 on the third day and pass it on the fourth day.</p><p>In the second example Vasiliy should prepare for the exam number 3 during the first four days and pass it on the fifth day. Then on the sixth day he should prepare for the exam number 2 and then pass it on the seventh day. After that he needs to prepare for the exam number 1 on the eighth day and pass it on the ninth day. </p><p>In the third example Vasiliy can't pass the only exam because he hasn't anough time to prepare for it. </p>
