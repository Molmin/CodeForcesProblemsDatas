## Description

<div><p>Recently <span class="tex-span"><i>n</i></span> students from city S moved to city P to attend a programming camp.</p><p>They moved there by train. In the evening, all students in the train decided that they want to drink some tea. Of course, no two people can use the same teapot simultaneously, so the students had to form a queue to get their tea.</p><p><span class="tex-span"><i>i</i></span>-th student comes to the end of the queue at the beginning of <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>-th second. If there are multiple students coming to the queue in the same moment, then the student with greater index comes after the student with lesser index. Students in the queue behave as follows: if there is nobody in the queue before the student, then he uses the teapot for exactly one second and leaves the queue with his tea; otherwise the student waits for the people before him to get their tea. If at the beginning of <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>-th second student <span class="tex-span"><i>i</i></span> still cannot get his tea (there is someone before him in the queue), then he leaves the queue without getting any tea. </p><p>For each student determine the second he will use the teapot and get his tea (if he actually gets it).</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>t</i></span> — the number of test cases to solve (<span class="tex-span">1 ≤ <i>t</i> ≤ 1000</span>).</p><p>Then <span class="tex-span"><i>t</i></span> test cases follow. The first line of each test case contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — the number of students.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow. Each line contains two integer <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 5000</span>) — the second <span class="tex-span"><i>i</i></span>-th student comes to the end of the queue, and the second he leaves the queue if he still cannot get his tea.</p><p>It is guaranteed that for every <img align="middle" class="tex-formula" src="file://QDzwcpFF.png" style="max-width: 100.0%;max-height: 100.0%;"> condition <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i> - 1</sub> ≤ <i>l</i><sub class="lower-index"><i>i</i></sub></span> holds.</p><p>The sum of <span class="tex-span"><i>n</i></span> over all test cases doesn't exceed <span class="tex-span">1000</span>.</p><p><span class="tex-font-style-bf">Note that in hacks you have to set <span class="tex-span"><i>t</i> = 1</span></span>.</p></div><div class="output-specification"><p>For each test case print <span class="tex-span"><i>n</i></span> integers. <span class="tex-span"><i>i</i></span>-th of them must be equal to the second when <span class="tex-span"><i>i</i></span>-th student gets his tea, or <span class="tex-span">0</span> if he leaves without tea.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>t</i></span> — the number of test cases to solve (<span class="tex-span">1 ≤ <i>t</i> ≤ 1000</span>).</p><p>Then <span class="tex-span"><i>t</i></span> test cases follow. The first line of each test case contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — the number of students.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow. Each line contains two integer <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 5000</span>) — the second <span class="tex-span"><i>i</i></span>-th student comes to the end of the queue, and the second he leaves the queue if he still cannot get his tea.</p><p>It is guaranteed that for every <img align="middle" class="tex-formula" src="file://QDzwcpFF.png" style="max-width: 100.0%;max-height: 100.0%;"> condition <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i> - 1</sub> ≤ <i>l</i><sub class="lower-index"><i>i</i></sub></span> holds.</p><p>The sum of <span class="tex-span"><i>n</i></span> over all test cases doesn't exceed <span class="tex-span">1000</span>.</p><p><span class="tex-font-style-bf">Note that in hacks you have to set <span class="tex-span"><i>t</i> = 1</span></span>.</p>

## Output

<p>For each test case print <span class="tex-span"><i>n</i></span> integers. <span class="tex-span"><i>i</i></span>-th of them must be equal to the second when <span class="tex-span"><i>i</i></span>-th student gets his tea, or <span class="tex-span">0</span> if he leaves without tea.</p>





```input1
2
2
1 3
1 4
3
1 5
1 1
2 3

```




```output1
1 2 
1 0 2 

```



## Note

<p>The example contains <span class="tex-span">2</span> tests:</p><ol> <li> During <span class="tex-span">1</span>-st second, students <span class="tex-span">1</span> and <span class="tex-span">2</span> come to the queue, and student <span class="tex-span">1</span> gets his tea. Student <span class="tex-span">2</span> gets his tea during <span class="tex-span">2</span>-nd second. </li><li> During <span class="tex-span">1</span>-st second, students <span class="tex-span">1</span> and <span class="tex-span">2</span> come to the queue, student <span class="tex-span">1</span> gets his tea, and student <span class="tex-span">2</span> leaves without tea. During <span class="tex-span">2</span>-nd second, student <span class="tex-span">3</span> comes and gets his tea. </li></ol>
