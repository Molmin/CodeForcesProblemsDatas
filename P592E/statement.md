## Description

<div><p>BCPC stands for Byteforces Collegiate Programming Contest, and is the most famous competition in Byteforces.</p><p>BCPC is a team competition. Each team is composed by a coach and three contestants. Blenda is the coach of the Bit State University(BSU), and she is very strict selecting the members of her team.</p><center> <img class="tex-graphics" src="file://RpE9i0PN.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In BSU there are <span class="tex-span"><i>n</i></span> students numbered from 1 to <span class="tex-span"><i>n</i></span>. Since all BSU students are infinitely smart, the only important parameters for Blenda are their reading and writing speed. After a careful measuring, Blenda have found that the <span class="tex-span"><i>i</i></span>-th student have a <span class="tex-font-style-bf">reading</span> speed equal to <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (words per minute), and a <span class="tex-font-style-bf">writing</span> speed of <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (symbols per minute). Since BSU students are very smart, the measured speeds are sometimes very big and Blenda have decided to subtract some constant value <span class="tex-span"><i>c</i></span> from all the values of reading speed and some value <span class="tex-span"><i>d</i></span> from all the values of writing speed. Therefore she considers <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub>' = <i>r</i><sub class="lower-index"><i>i</i></sub> - <i>c</i></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub>' = <i>w</i><sub class="lower-index"><i>i</i></sub> - <i>d</i></span>. </p><p>The student <span class="tex-span"><i>i</i></span> is said to <span class="tex-font-style-it">overwhelm</span> the student <span class="tex-span"><i>j</i></span> if and only if <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub>'·<i>w</i><sub class="lower-index"><i>j</i></sub>' &gt; <i>r</i><sub class="lower-index"><i>j</i></sub>'·<i>w</i><sub class="lower-index"><i>i</i></sub>'</span>. Blenda doesn’t like fights in teams, so she thinks that a team consisting of three distinct students <span class="tex-span"><i>i</i>, <i>j</i></span> and <span class="tex-span"><i>k</i></span> is <span class="tex-font-style-it">good</span> if <span class="tex-span"><i>i</i></span> overwhelms <span class="tex-span"><i>j</i></span>, <span class="tex-span"><i>j</i></span> overwhelms <span class="tex-span"><i>k</i></span>, and <span class="tex-span"><i>k</i></span> overwhelms <span class="tex-span"><i>i</i></span>. Yes, the relation of overwhelming is not transitive as it often happens in real life.</p><p>Since Blenda is busy preparing a training camp in Codeforces, you are given a task to calculate the number of different good teams in BSU. Two teams are considered to be different if there is at least one student that is present in one team but is not present in the other. In other words, two teams are different if the sets of students that form these teams are different.</p></div><div class="input-specification"><p>In the first line of the input three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>c</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 345678, 1 ≤ <i>c</i>, <i>d</i> ≤ 10<sup class="upper-index">9</sup></span>) are written. They denote the number of students Blenda can use to form teams, the value subtracted from all reading speeds and the value subtracted from all writing speeds respectively.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 &lt; <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>, |<i>r</i><sub class="lower-index"><i>i</i></sub> - <i>c</i>| + |<i>w</i><sub class="lower-index"><i>i</i></sub> - <i>d</i>| &gt; 0</span>). There are no two students, such that both their reading and writing speeds coincide, i.e. for every <span class="tex-span"><i>i</i> ≠ <i>j</i></span> condition <span class="tex-span">|<i>r</i><sub class="lower-index"><i>i</i></sub> - <i>r</i><sub class="lower-index"><i>j</i></sub>| + |<i>w</i><sub class="lower-index"><i>i</i></sub> - <i>w</i><sub class="lower-index"><i>j</i></sub>| &gt; 0</span> holds.</p></div><div class="output-specification"><p>Print the number of different teams in BSU, that are good according to Blenda's definition.</p></div>

## Input

<p>In the first line of the input three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>c</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 345678, 1 ≤ <i>c</i>, <i>d</i> ≤ 10<sup class="upper-index">9</sup></span>) are written. They denote the number of students Blenda can use to form teams, the value subtracted from all reading speeds and the value subtracted from all writing speeds respectively.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 &lt; <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>, |<i>r</i><sub class="lower-index"><i>i</i></sub> - <i>c</i>| + |<i>w</i><sub class="lower-index"><i>i</i></sub> - <i>d</i>| &gt; 0</span>). There are no two students, such that both their reading and writing speeds coincide, i.e. for every <span class="tex-span"><i>i</i> ≠ <i>j</i></span> condition <span class="tex-span">|<i>r</i><sub class="lower-index"><i>i</i></sub> - <i>r</i><sub class="lower-index"><i>j</i></sub>| + |<i>w</i><sub class="lower-index"><i>i</i></sub> - <i>w</i><sub class="lower-index"><i>j</i></sub>| &gt; 0</span> holds.</p>

## Output

<p>Print the number of different teams in BSU, that are good according to Blenda's definition.</p>





```input1
5 2 2
1 1
4 1
2 3
3 2
3 4

```




```input2
7 6 6
3 2
1 7
5 7
3 7
6 4
8 9
8 5

```




```output1
4

```




```output2
11

```



## Note

<p>In the first sample the following teams are good: <span class="tex-span">(<i>i</i> = 1, <i>j</i> = 2, <i>k</i> = 3)</span>, <span class="tex-span">(<i>i</i> = 2, <i>j</i> = 5, <i>k</i> = 1)</span>, <span class="tex-span">(<i>i</i> = 1, <i>j</i> = 4, <i>k</i> = 3)</span>, <span class="tex-span">(<i>i</i> = 5, <i>j</i> = 1, <i>k</i> = 4)</span>.</p><p>Note, that for example the team <span class="tex-span">(<i>i</i> = 3, <i>j</i> = 1, <i>k</i> = 2)</span> is also good, but is considered to be the same as the team <span class="tex-span">(<i>i</i> = 1, <i>j</i> = 2, <i>k</i> = 3)</span>.</p>
