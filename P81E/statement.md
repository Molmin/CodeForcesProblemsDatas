## Description

<div><p>There are <span class="tex-span"><i>n</i></span> students in Polycarp's class (including himself). A few days ago all students wrote an essay "My best friend". Each student's essay was dedicated to one of the students of class, to his/her best friend. Note that student <span class="tex-span"><i>b</i></span>'s best friend is not necessarily student <span class="tex-span"><i>a</i></span>, if <span class="tex-span"><i>a</i></span>'s best friend is <span class="tex-span"><i>b</i></span>.</p><p>And now the teacher leads the whole class to the museum of the history of sports programming. Exciting stories of legendary heroes await the students: tourist, Petr, tomek, SnapDragon — that's who they will hear about!</p><p>The teacher decided to divide students into pairs so that each pair consisted of a student and his best friend. She may not be able to split all the students into pairs, it's not a problem — she wants to pick out the maximum number of such pairs. If there is more than one variant of doing so, she wants to pick out the pairs so that there were as much boy-girl pairs as possible. Of course, each student must not be included in more than one pair.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), <span class="tex-span"><i>n</i></span> is the number of students per class. Next, <span class="tex-span"><i>n</i></span> lines contain information about the students, one per line. Each line contains two integers <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub>, <i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>f</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>f</i><sub class="lower-index"><i>i</i></sub> ≠ <i>i</i>, 1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>), where <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> is the number of <span class="tex-span"><i>i</i></span>-th student's best friend and <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> denotes the <span class="tex-span"><i>i</i></span>-th pupil's sex (<span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> = 1</span> for a boy and <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> = 2</span> for a girl).</p></div><div class="output-specification"><p>Print on the first line two numbers <span class="tex-span"><i>t</i></span>, <span class="tex-span"><i>e</i></span>, where <span class="tex-span"><i>t</i></span> is the maximum number of formed pairs, and <span class="tex-span"><i>e</i></span> is the maximum number of boy-girl type pairs among them. Then print <span class="tex-span"><i>t</i></span> lines, each line must contain a pair <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), they are numbers of pupils in the <span class="tex-span"><i>i</i></span>-th pair. Print the pairs in any order. Print the numbers in pairs in any order. If there are several solutions, output any of them.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), <span class="tex-span"><i>n</i></span> is the number of students per class. Next, <span class="tex-span"><i>n</i></span> lines contain information about the students, one per line. Each line contains two integers <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub>, <i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>f</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>f</i><sub class="lower-index"><i>i</i></sub> ≠ <i>i</i>, 1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>), where <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> is the number of <span class="tex-span"><i>i</i></span>-th student's best friend and <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> denotes the <span class="tex-span"><i>i</i></span>-th pupil's sex (<span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> = 1</span> for a boy and <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> = 2</span> for a girl).</p>

## Output

<p>Print on the first line two numbers <span class="tex-span"><i>t</i></span>, <span class="tex-span"><i>e</i></span>, where <span class="tex-span"><i>t</i></span> is the maximum number of formed pairs, and <span class="tex-span"><i>e</i></span> is the maximum number of boy-girl type pairs among them. Then print <span class="tex-span"><i>t</i></span> lines, each line must contain a pair <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), they are numbers of pupils in the <span class="tex-span"><i>i</i></span>-th pair. Print the pairs in any order. Print the numbers in pairs in any order. If there are several solutions, output any of them.</p>





```input1
5
5 2
3 2
5 1
2 1
4 2

```




```input2
6
5 2
3 2
5 1
2 1
4 2
3 1

```




```input3
8
2 2
3 2
5 1
3 1
6 1
5 1
8 2
7 1

```




```output1
2 2
5 3
4 2

```




```output2
3 1
4 2
5 1
3 6

```




```output3
4 1
5 6
3 4
2 1
7 8

```



## Note

<p>The picture corresponds to the first sample. On the picture rhomb stand for boys, squares stand for girls, arrows lead from a pupil to his/her best friend. Bold non-dashed arrows stand for pairs in the answer. </p><center> <img class="tex-graphics" src="file://IJSOfhsE.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
