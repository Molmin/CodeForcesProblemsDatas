## Description

<div><p>Professor GukiZ likes programming contests. He especially likes to rate his students on the contests he prepares. Now, he has decided to prepare a new contest. </p><p>In total, <span class="tex-span"><i>n</i></span> students will attend, and before the start, every one of them has some positive integer rating. Students are indexed from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Let's denote the rating of <span class="tex-span"><i>i</i></span>-th student as <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. After the contest ends, every student will end up with some positive integer position. GukiZ expects that his students will take places according to their ratings. </p><p>He thinks that each student will take place equal to <img align="middle" class="tex-formula" src="file://D6ftgAOc.png" style="max-width: 100.0%;max-height: 100.0%;">. In particular, if student <span class="tex-span"><i>A</i></span> has rating strictly lower then student <span class="tex-span"><i>B</i></span>, <span class="tex-span"><i>A</i></span> will get the strictly better position than <span class="tex-span"><i>B</i></span>, and if two students have equal ratings, they will share the same position. </p><p>GukiZ would like you to reconstruct the results by following his expectations. Help him and determine the position after the end of the contest for each of his students if everything goes as expected.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>), number of GukiZ's students. </p><p>The second line contains <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 2000</span>) where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the rating of <span class="tex-span"><i>i</i></span>-th student (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>).</p></div><div class="output-specification"><p>In a single line, print the position after the end of the contest for each of <span class="tex-span"><i>n</i></span> students in the same order as they appear in the input.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>), number of GukiZ's students. </p><p>The second line contains <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 2000</span>) where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the rating of <span class="tex-span"><i>i</i></span>-th student (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>).</p>

## Output

<p>In a single line, print the position after the end of the contest for each of <span class="tex-span"><i>n</i></span> students in the same order as they appear in the input.</p>





```input1
3
1 3 3

```




```input2
1
1

```




```input3
5
3 5 3 4 5

```




```output1
3 1 1

```




```output2
1

```




```output3
4 1 4 3 1

```



## Note

<p>In the first sample, students <span class="tex-span">2</span> and <span class="tex-span">3</span> are positioned first (there is no other student with higher rating), and student <span class="tex-span">1</span> is positioned third since there are two students with higher rating.</p><p>In the second sample, first student is the only one on the contest.</p><p>In the third sample, students <span class="tex-span">2</span> and <span class="tex-span">5</span> share the first position with highest rating, student <span class="tex-span">4</span> is next with third position, and students <span class="tex-span">1</span> and <span class="tex-span">3</span> are the last sharing fourth position.</p>
