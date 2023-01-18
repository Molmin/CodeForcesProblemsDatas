## Description

<div><p>Instructors of Some Informatics School make students go to bed.</p><p>The house contains <span class="tex-span"><i>n</i></span> rooms, in each room exactly <span class="tex-span"><i>b</i></span> students were supposed to sleep. However, at the time of curfew it happened that many students are not located in their assigned rooms. The rooms are arranged in a row and numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Initially, in <span class="tex-span"><i>i</i></span>-th room there are <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> students. All students are currently somewhere in the house, therefore <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> + <i>a</i><sub class="lower-index">2</sub> + ... + <i>a</i><sub class="lower-index"><i>n</i></sub> = <i>nb</i></span>. Also <span class="tex-span">2</span> instructors live in this house.</p><p>The process of curfew enforcement is the following. One instructor starts near room <span class="tex-span">1</span> and moves toward room <span class="tex-span"><i>n</i></span>, while the second instructor starts near room <span class="tex-span"><i>n</i></span> and moves toward room <span class="tex-span">1</span>. After processing current room, each instructor moves on to the next one. Both instructors enter rooms and move simultaneously, if <span class="tex-span"><i>n</i></span> is odd, then only the first instructor processes the middle room. When all rooms are processed, the process ends.</p><p>When an instructor processes a room, she counts the number of students in the room, then turns off the light, and locks the room. Also, if the number of students inside the processed room is not equal to <span class="tex-span"><i>b</i></span>, the instructor writes down the number of this room into her notebook (and turns off the light, and locks the room). Instructors are in a hurry (to prepare the study plan for the next day), so they don't care about who is in the room, but only about the number of students.</p><p>While instructors are inside the rooms, students can run between rooms that are not locked and not being processed. A student can run by at most <span class="tex-span"><i>d</i></span> rooms, that is she can move to a room with number that differs my at most <span class="tex-span"><i>d</i></span>. Also, after (or instead of) running each student can hide under a bed in a room she is in. In this case the instructor will not count her during the processing. In each room any number of students can hide simultaneously.</p><p>Formally, here is what's happening:</p><ul> <li> A curfew is announced, at this point in room <span class="tex-span"><i>i</i></span> there are <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> students. </li><li> Each student can run to another room but not further than <span class="tex-span"><i>d</i></span> rooms away from her initial room, or stay in place. After that each student can optionally hide under a bed. </li><li> Instructors enter room <span class="tex-span">1</span> and room <span class="tex-span"><i>n</i></span>, they count students there and lock the room (after it no one can enter or leave this room). </li><li> Each student from rooms with numbers from <span class="tex-span">2</span> to <span class="tex-span"><i>n</i> - 1</span> can run to another room but not further than <span class="tex-span"><i>d</i></span> rooms away from her <span class="tex-font-style-bf">current</span> room, or stay in place. Each student can optionally hide under a bed. </li><li> Instructors move from room <span class="tex-span">1</span> to room <span class="tex-span">2</span> and from room <span class="tex-span"><i>n</i></span> to room <span class="tex-span"><i>n</i> - 1</span>. </li><li> This process continues until all rooms are processed. </li></ul><p>Let <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> denote the number of rooms in which the first instructor counted the number of non-hidden students different from <span class="tex-span"><i>b</i></span>, and <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> be the same number for the second instructor. Students know that the principal will only listen to one complaint, therefore they want to minimize the maximum of numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>. Help them find this value if they use the optimal strategy.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>d</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>d</i> ≤ <i>n</i> - 1</span>, <span class="tex-span">1 ≤ <i>b</i> ≤ 10 000</span>), number of rooms in the house, running distance of a student, official number of students in a room.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), <span class="tex-span"><i>i</i></span>-th of which stands for the number of students in the <span class="tex-span"><i>i</i></span>-th room before curfew announcement.</p><p>It is guaranteed that <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> + <i>a</i><sub class="lower-index">2</sub> + ... + <i>a</i><sub class="lower-index"><i>n</i></sub> = <i>nb</i></span>.</p></div><div class="output-specification"><p>Output one integer, the minimal possible value of the maximum of <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>d</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>d</i> ≤ <i>n</i> - 1</span>, <span class="tex-span">1 ≤ <i>b</i> ≤ 10 000</span>), number of rooms in the house, running distance of a student, official number of students in a room.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), <span class="tex-span"><i>i</i></span>-th of which stands for the number of students in the <span class="tex-span"><i>i</i></span>-th room before curfew announcement.</p><p>It is guaranteed that <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> + <i>a</i><sub class="lower-index">2</sub> + ... + <i>a</i><sub class="lower-index"><i>n</i></sub> = <i>nb</i></span>.</p>

## Output

<p>Output one integer, the minimal possible value of the maximum of <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>.</p>





```input1
5 1 1
1 0 0 0 4

```




```input2
6 1 2
3 8 0 1 0 0

```




```output1
1

```




```output2
2

```



## Note

<p>In the first sample the first three rooms are processed by the first instructor, and the last two are processed by the second instructor. One of the optimal strategies is the following: firstly three students run from room <span class="tex-span">5</span> to room <span class="tex-span">4</span>, on the next stage two of them run to room <span class="tex-span">3</span>, and one of those two hides under a bed. This way, the first instructor writes down room <span class="tex-span">2</span>, and the second writes down nothing.</p><p>In the second sample one of the optimal strategies is the following: firstly all students in room <span class="tex-span">1</span> hide, all students from room <span class="tex-span">2</span> run to room <span class="tex-span">3</span>. On the next stage one student runs from room <span class="tex-span">3</span> to room <span class="tex-span">4</span>, and <span class="tex-span">5</span> students hide. This way, the first instructor writes down rooms <span class="tex-span">1</span> and <span class="tex-span">2</span>, the second instructor writes down rooms <span class="tex-span">5</span> and <span class="tex-span">6</span>.</p>
