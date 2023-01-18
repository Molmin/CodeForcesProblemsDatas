## Description

<div><p>Student Valera is an undergraduate student at the University. His end of term exams are approaching and he is to pass exactly <span class="tex-span"><i>n</i></span> exams. Valera is a smart guy, so he will be able to pass any exam he takes on his first try. Besides, he can take several exams on one day, and in any order.</p><p>According to the schedule, a student can take the exam for the <span class="tex-span"><i>i</i></span>-th subject on the day number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. However, Valera has made an arrangement with each teacher and the teacher of the <span class="tex-span"><i>i</i></span>-th subject allowed him to take an exam before the schedule time on day <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> &lt; <i>a</i><sub class="lower-index"><i>i</i></sub></span>). Thus, Valera can take an exam for the <span class="tex-span"><i>i</i></span>-th subject either on day <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, or on day <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. All the teachers put the record of the exam in the student's record book on the day of the actual exam and write down the date of the mark as number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Valera believes that it would be rather strange if the entries in the record book did not go in the order of non-decreasing date. Therefore Valera asks you to help him. Find the minimum possible value of the day when Valera can take the final exam if he takes exams so that all the records in his record book go in the order of non-decreasing date.</p></div><div class="input-specification"><p>The first line contains a single positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>) — the number of exams Valera will take.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two positive space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> &lt; <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the date of the exam in the schedule and the early date of passing the <span class="tex-span"><i>i</i></span>-th exam, correspondingly.</p></div><div class="output-specification"><p>Print a single integer — the minimum possible number of the day when Valera can take the last exam if he takes all the exams so that all the records in his record book go in the order of non-decreasing date.</p></div>

## Input

<p>The first line contains a single positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>) — the number of exams Valera will take.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two positive space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> &lt; <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the date of the exam in the schedule and the early date of passing the <span class="tex-span"><i>i</i></span>-th exam, correspondingly.</p>

## Output

<p>Print a single integer — the minimum possible number of the day when Valera can take the last exam if he takes all the exams so that all the records in his record book go in the order of non-decreasing date.</p>





```input1
3
5 2
3 1
4 2

```




```input2
3
6 1
5 2
4 3

```




```output1
2

```




```output2
6

```



## Note

<p>In the first sample Valera first takes an exam in the second subject on the first day (the teacher writes down the schedule date that is 3). On the next day he takes an exam in the third subject (the teacher writes down the schedule date, 4), then he takes an exam in the first subject (the teacher writes down the mark with date 5). Thus, Valera takes the last exam on the second day and the dates will go in the non-decreasing order: 3, 4, 5.</p><p>In the second sample Valera first takes an exam in the third subject on the fourth day. Then he takes an exam in the second subject on the fifth day. After that on the sixth day Valera takes an exam in the first subject.</p>
