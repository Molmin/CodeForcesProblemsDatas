## Description

<div><p>Yet another education system reform has been carried out in Berland recently. The innovations are as follows:</p><p>An academic year now consists of <span class="tex-span"><i>n</i></span> days. Each day pupils study exactly one of <span class="tex-span"><i>m</i></span> subjects, besides, each subject is studied for no more than one day. After the lessons of the <span class="tex-span"><i>i</i></span>-th subject pupils get the home task that contains no less than <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and no more than <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> exercises. Besides, each subject has a special attribute, the complexity (<span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>). A school can make its own timetable, considering the following conditions are satisfied:</p><ul> <li> the timetable should contain the subjects in the order of the complexity's strict increasing; </li><li> each day, except for the first one, the task should contain either <span class="tex-span"><i>k</i></span> times more exercises, or more by <span class="tex-span"><i>k</i></span> compared to the previous day (more formally: let's call the number of home task exercises in the <span class="tex-span"><i>i</i></span>-th day as <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, then for each <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 &lt; <i>i</i> ≤ <i>n</i></span>): either <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> = <i>k</i> + <i>x</i><sub class="lower-index"><i>i</i> - 1</sub></span> or <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> = <i>k</i>·<i>x</i><sub class="lower-index"><i>i</i> - 1</sub></span> must be true); </li><li> the total number of exercises in all home tasks should be maximal possible. </li></ul><p>All limitations are separately set for each school.</p><p>It turned out that in many cases <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> reach <span class="tex-span">10<sup class="upper-index">16</sup></span> (however, as the Berland Minister of Education is famous for his love to half-measures, the value of <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> - <i>a</i><sub class="lower-index"><i>i</i></sub></span> doesn't exceed <span class="tex-span">100</span>). That also happened in the Berland School №256. Nevertheless, you as the school's principal still have to work out the timetable for the next academic year...</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ <i>m</i> ≤ 50</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 100</span>) which represent the number of days in an academic year, the number of subjects and the <span class="tex-span"><i>k</i></span> parameter correspondingly. Each of the following <span class="tex-span"><i>m</i></span> lines contains the description of a subject as three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">16</sup></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> - <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — two limitations to the number of exercises on the <span class="tex-span"><i>i</i></span>-th subject and the complexity of the <span class="tex-span"><i>i</i></span>-th subject, correspondingly. Distinct subjects can have the same complexity. The subjects are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>. </p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit numbers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span> stream or the <span class="tex-font-style-tt">%I64d</span> specificator.</p></div><div class="output-specification"><p>If no valid solution exists, print the single word "<span class="tex-font-style-tt">NO</span>" (without the quotes). Otherwise, the first line should contain the word "<span class="tex-font-style-tt">YES</span>" (without the quotes) and the next <span class="tex-span"><i>n</i></span> lines should contain any timetable that satisfies all the conditions. The <span class="tex-span"><i>i</i> + 1</span>-th line should contain two positive integers: the number of the subject to study on the <span class="tex-span"><i>i</i></span>-th day and the number of home task exercises given for this subject. The timetable should contain exactly <span class="tex-span"><i>n</i></span> subjects.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ <i>m</i> ≤ 50</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 100</span>) which represent the number of days in an academic year, the number of subjects and the <span class="tex-span"><i>k</i></span> parameter correspondingly. Each of the following <span class="tex-span"><i>m</i></span> lines contains the description of a subject as three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">16</sup></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> - <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — two limitations to the number of exercises on the <span class="tex-span"><i>i</i></span>-th subject and the complexity of the <span class="tex-span"><i>i</i></span>-th subject, correspondingly. Distinct subjects can have the same complexity. The subjects are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>. </p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit numbers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span> stream or the <span class="tex-font-style-tt">%I64d</span> specificator.</p>

## Output

<p>If no valid solution exists, print the single word "<span class="tex-font-style-tt">NO</span>" (without the quotes). Otherwise, the first line should contain the word "<span class="tex-font-style-tt">YES</span>" (without the quotes) and the next <span class="tex-span"><i>n</i></span> lines should contain any timetable that satisfies all the conditions. The <span class="tex-span"><i>i</i> + 1</span>-th line should contain two positive integers: the number of the subject to study on the <span class="tex-span"><i>i</i></span>-th day and the number of home task exercises given for this subject. The timetable should contain exactly <span class="tex-span"><i>n</i></span> subjects.</p>





```input1
4 5 2
1 10 1
1 10 2
1 10 3
1 20 4
1 100 5

```




```input2
3 4 3
1 3 1
2 4 4
2 3 3
2 2 2

```




```output1
YES
2 8
3 10
4 20
5 40

```




```output2
NO
```


