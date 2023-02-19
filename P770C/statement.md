## Description

<div><p>Now you can take online courses in the Berland State University! Polycarp needs to pass <span class="tex-span"><i>k</i></span> <span class="tex-font-style-bf">main</span> online courses of his specialty to get a diploma. In total <span class="tex-span"><i>n</i></span> courses are availiable for the passage.</p><p>The situation is complicated by the dependence of online courses, for each course there is a list of those that must be passed before starting this online course (the list can be empty, it means that there is no limitation).</p><p>Help Polycarp to pass the least number of courses in total to get the specialty (it means to pass all <span class="tex-font-style-bf">main</span> and necessary courses). Write a program which prints the order of courses. </p><p>Polycarp passes courses consistently, he starts the next course when he finishes the previous one. Each course can't be passed more than once. </p></div><div class="input-specification"><p>The first line contains <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of online-courses and the number of main courses of Polycarp's specialty. </p><p>The second line contains <span class="tex-span"><i>k</i></span> distinct integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> — numbers of main online-courses of Polycarp's specialty. </p><p>Then <span class="tex-span"><i>n</i></span> lines follow, each of them describes the next course: the <span class="tex-span"><i>i</i></span>-th of them corresponds to the course <span class="tex-span"><i>i</i></span>. Each line starts from the integer <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - 1</span>) — the number of courses on which the <span class="tex-span"><i>i</i></span>-th depends. Then there follows the sequence of <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> distinct integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> — numbers of courses in random order, on which the <span class="tex-span"><i>i</i></span>-th depends. It is guaranteed that no course can depend on itself. </p><p>It is guaranteed that the sum of all values <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>. </p></div><div class="output-specification"><p>Print <span class="tex-font-style-tt">-1</span>, if there is no the way to get a specialty. </p><p>Otherwise, in the first line print the integer <span class="tex-span"><i>m</i></span> — the minimum number of online-courses which it is necessary to pass to get a specialty. In the second line print <span class="tex-span"><i>m</i></span> distinct integers — numbers of courses which it is necessary to pass in the chronological order of their passage. If there are several answers it is allowed to print any of them.</p></div>

## Input

<p>The first line contains <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of online-courses and the number of main courses of Polycarp's specialty. </p><p>The second line contains <span class="tex-span"><i>k</i></span> distinct integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> — numbers of main online-courses of Polycarp's specialty. </p><p>Then <span class="tex-span"><i>n</i></span> lines follow, each of them describes the next course: the <span class="tex-span"><i>i</i></span>-th of them corresponds to the course <span class="tex-span"><i>i</i></span>. Each line starts from the integer <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - 1</span>) — the number of courses on which the <span class="tex-span"><i>i</i></span>-th depends. Then there follows the sequence of <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> distinct integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> — numbers of courses in random order, on which the <span class="tex-span"><i>i</i></span>-th depends. It is guaranteed that no course can depend on itself. </p><p>It is guaranteed that the sum of all values <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>. </p>

## Output

<p>Print <span class="tex-font-style-tt">-1</span>, if there is no the way to get a specialty. </p><p>Otherwise, in the first line print the integer <span class="tex-span"><i>m</i></span> — the minimum number of online-courses which it is necessary to pass to get a specialty. In the second line print <span class="tex-span"><i>m</i></span> distinct integers — numbers of courses which it is necessary to pass in the chronological order of their passage. If there are several answers it is allowed to print any of them.</p>





```input1
6 2
5 3
0
0
0
2 2 1
1 4
1 5

```




```input2
9 3
3 9 5
0
0
3 9 4 5
0
0
1 8
1 6
1 2
2 1 2

```




```input3
3 3
1 2 3
1 2
1 3
1 1

```




```output1
5
1 2 3 4 5 

```




```output2
6
1 2 9 4 5 3 

```




```output3
-1

```



## Note

<p>In the first test firstly you can take courses number <span class="tex-span">1</span> and <span class="tex-span">2</span>, after that you can take the course number <span class="tex-span">4</span>, then you can take the course number <span class="tex-span">5</span>, which is the main. After that you have to take only the course number <span class="tex-span">3</span>, which is the last not passed main course. </p>
