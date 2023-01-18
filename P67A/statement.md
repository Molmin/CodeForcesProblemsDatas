## Description

<div><p>A teacher decides to give toffees to his students. He asks <span class="tex-span"><i>n</i></span> students to stand in a queue. Since the teacher is very partial, he follows the following rule to distribute toffees.</p><p>He looks at the first two students and gives more toffees to the student having higher marks than the other one. If they have the same marks they get the same number of toffees. The same procedure is followed for each pair of adjacent students starting from the first one to the last one.</p><p>It is given that each student receives at least one toffee. You have to find the number of toffees given to each student by the teacher such that the total number of toffees is minimum.</p></div><div class="input-specification"><p>The first line of input contains the number of students <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>). The second line gives (<span class="tex-span"><i>n</i> - 1</span>) characters consisting of "<span class="tex-font-style-tt">L</span>", "<span class="tex-font-style-tt">R</span>" and "<span class="tex-font-style-tt">=</span>". For each pair of adjacent students "<span class="tex-font-style-tt">L</span>" means that the left student has higher marks, "<span class="tex-font-style-tt">R</span>" means that the right student has higher marks and "<span class="tex-font-style-tt">=</span>" means that both have equal marks. </p></div><div class="output-specification"><p>Output consists of <span class="tex-span"><i>n</i></span> integers separated by a space representing the number of toffees each student receives in the queue starting from the first one to the last one.</p></div>

## Input

<p>The first line of input contains the number of students <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>). The second line gives (<span class="tex-span"><i>n</i> - 1</span>) characters consisting of "<span class="tex-font-style-tt">L</span>", "<span class="tex-font-style-tt">R</span>" and "<span class="tex-font-style-tt">=</span>". For each pair of adjacent students "<span class="tex-font-style-tt">L</span>" means that the left student has higher marks, "<span class="tex-font-style-tt">R</span>" means that the right student has higher marks and "<span class="tex-font-style-tt">=</span>" means that both have equal marks. </p>

## Output

<p>Output consists of <span class="tex-span"><i>n</i></span> integers separated by a space representing the number of toffees each student receives in the queue starting from the first one to the last one.</p>





```input1
5
LRLR

```




```input2
5
=RRR

```




```output1
2 1 2 1 2

```




```output2
1 1 2 3 4

```


