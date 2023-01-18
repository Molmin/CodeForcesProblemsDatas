## Description

<div><p>Vasya, or Mr. Vasily Petrov is a dean of a department in a local university. After the winter exams he got his hands on a group's gradebook.</p><p>Overall the group has <span class="tex-span"><i>n</i></span> students. They received marks for <span class="tex-span"><i>m</i></span> subjects. Each student got a mark from <span class="tex-span">1</span> to <span class="tex-span">9</span> (inclusive) for each subject.</p><p>Let's consider a student the <span class="tex-font-style-it">best at some subject</span>, if there is no student who got a higher mark for this subject. Let's consider a student <span class="tex-font-style-it">successful</span>, if there exists a subject he is the <span class="tex-font-style-it">best at</span>.</p><p>Your task is to find the number of <span class="tex-font-style-it">successful</span> students in the group.</p></div><div class="input-specification"><p>The first input line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>) — the number of students and the number of subjects, correspondingly. Next <span class="tex-span"><i>n</i></span> lines each containing <span class="tex-span"><i>m</i></span> characters describe the gradebook. Each character in the gradebook is a number from <span class="tex-span">1</span> to <span class="tex-span">9</span>. Note that the marks in a rows are not sepatated by spaces.</p></div><div class="output-specification"><p>Print the single number — the number of <span class="tex-font-style-it">successful</span> students in the given group.</p></div>

## Input

<p>The first input line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>) — the number of students and the number of subjects, correspondingly. Next <span class="tex-span"><i>n</i></span> lines each containing <span class="tex-span"><i>m</i></span> characters describe the gradebook. Each character in the gradebook is a number from <span class="tex-span">1</span> to <span class="tex-span">9</span>. Note that the marks in a rows are not sepatated by spaces.</p>

## Output

<p>Print the single number — the number of <span class="tex-font-style-it">successful</span> students in the given group.</p>





```input1
3 3
223
232
112

```




```input2
3 5
91728
11828
11111

```




```output1
2

```




```output2
3

```



## Note

<p>In the first sample test the student number <span class="tex-span">1</span> is the best at subjects <span class="tex-span">1</span> and <span class="tex-span">3</span>, student <span class="tex-span">2</span> is the best at subjects <span class="tex-span">1</span> and <span class="tex-span">2</span>, but student <span class="tex-span">3</span> isn't the best at any subject.</p><p>In the second sample test each student is the best at at least one subject.</p>
