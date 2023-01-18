## Description

<div><p>An exam for <span class="tex-span"><i>n</i></span> students will take place in a long and narrow room, so the students will sit in a line in some order. The teacher suspects that students with adjacent numbers (<span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>i</i> + 1</span>) always studied side by side and became friends and if they take an exam sitting next to each other, they will help each other for sure.</p><p>Your task is to choose the maximum number of students and make such an arrangement of students in the room that no two students with adjacent numbers sit side by side.</p></div><div class="input-specification"><p>A single line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>) — the number of students at an exam.</p></div><div class="output-specification"><p>In the first line print integer <span class="tex-span"><i>k</i></span> — the maximum number of students who can be seated so that no two students with adjacent numbers sit next to each other.</p><p>In the second line print <span class="tex-span"><i>k</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of the student on the <span class="tex-span"><i>i</i></span>-th position. The students on adjacent positions mustn't have adjacent numbers. Formally, the following should be true: <span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub> - <i>a</i><sub class="lower-index"><i>i</i> + 1</sub>| ≠ 1</span> for all <span class="tex-span"><i>i</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i> - 1</span>.</p><p><span class="tex-font-style-bf">If there are several possible answers, output any of them.</span></p></div>

## Input

<p>A single line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>) — the number of students at an exam.</p>

## Output

<p>In the first line print integer <span class="tex-span"><i>k</i></span> — the maximum number of students who can be seated so that no two students with adjacent numbers sit next to each other.</p><p>In the second line print <span class="tex-span"><i>k</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of the student on the <span class="tex-span"><i>i</i></span>-th position. The students on adjacent positions mustn't have adjacent numbers. Formally, the following should be true: <span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub> - <i>a</i><sub class="lower-index"><i>i</i> + 1</sub>| ≠ 1</span> for all <span class="tex-span"><i>i</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i> - 1</span>.</p><p><span class="tex-font-style-bf">If there are several possible answers, output any of them.</span></p>





```input1
6
```




```input2
3

```




```output1
6
1 5 3 6 2 4
```




```output2
2
1 3
```


