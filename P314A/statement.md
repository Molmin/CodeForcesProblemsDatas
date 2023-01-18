## Description

<div><p>During the last Sereja's Codesecrof round the server crashed many times, so the round was decided to be made unrated for some participants. </p><p>Let's assume that <span class="tex-span"><i>n</i></span> people took part in the contest. Let's assume that the participant who got the first place has rating <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, the second place participant has rating <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, the <span class="tex-span"><i>n</i></span>-th place participant has rating <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span>. Then changing the rating on the Codesecrof site is calculated by the formula <img align="middle" class="tex-formula" src="file://PfqMW468.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>After the round was over, the Codesecrof management published the participants' results table. They decided that if for a participant <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub> &lt; <i>k</i></span>, then the round can be considered unrated for him. But imagine the management's surprise when they found out that the participants' rating table is dynamic. In other words, when some participant is removed from the rating, he is removed from the results' table and the rating is recalculated according to the new table. And of course, all applications for exclusion from the rating are considered in view of the current table.</p><p>We know that among all the applications for exclusion from the rating the first application to consider is from the participant with the best rank (the rank with the minimum number), for who <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub> &lt; <i>k</i></span>. We also know that the applications for exclusion from rating were submitted by all participants.</p><p>Now Sereja wonders, what is the number of participants to be excluded from the contest rating, and the numbers of the participants in the original table in the order of their exclusion from the rating. Pay attention to the analysis of the first test case for a better understanding of the statement.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup>,  - 10<sup class="upper-index">9</sup> ≤ <i>k</i> ≤ 0)</span>. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — ratings of the participants in the initial table.</p></div><div class="output-specification"><p>Print the numbers of participants in the order in which they were removed from the table. Print the initial numbers of the participants, that is, the numbers that the participants had in the initial table.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup>,  - 10<sup class="upper-index">9</sup> ≤ <i>k</i> ≤ 0)</span>. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — ratings of the participants in the initial table.</p>

## Output

<p>Print the numbers of participants in the order in which they were removed from the table. Print the initial numbers of the participants, that is, the numbers that the participants had in the initial table.</p>





```input1
5 0
5 3 4 1 2

```




```input2
10 -10
5 5 1 7 5 1 2 4 9 2

```




```output1
2
3
4

```




```output2
2
4
5
7
8
9

```



## Note

<p>Consider the first test sample. </p><ol><li> Initially the sequence of the contest participants' ratings equals [5, 3, 4, 1, 2]. You can use this sequence to calculate the sequence of rating changes: [0, -9, -13, 8, 14]. According to the problem statement, the application of the participant who won the second place will be considered first.</li><li> As soon as the second place winner is out from the ratings, the participants' rating sequence will equal [5, 4, 1, 2]. By this sequence you can count the new sequence of rating changes: [0, -8, 2, 6]. According to the problem statement, the application of the participant who won the second place will be considered. Initially this participant won third place.</li><li> The new rating sequence equals [5, 1, 2], the new sequence of rating changes equals [0, -1, 1]. The second place participant's application is taken into consideration, initially this participant won the fourth place.</li><li> The new rating sequence equals [5, 2], the new sequence of rating changes equals [0, 0]. No more applications will be considered. </li></ol><p>Thus, you should print 2, 3, 4.</p>
