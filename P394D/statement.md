## Description

<div><p>The Physical education teacher at SESC is a sort of mathematician too. His most favorite topic in mathematics is progressions. That is why the teacher wants the students lined up in <span class="tex-font-style-bf">non-decreasing</span> height form an arithmetic progression.</p><p>To achieve the goal, the gym teacher ordered a lot of magical buns from the dining room. The magic buns come in two types: when a student eats one magic bun of the first type, his height increases by one, when the student eats one magical bun of the second type, his height decreases by one. The physical education teacher, as expected, cares about the health of his students, so he does not want them to eat a lot of buns. More precisely, he wants the maximum number of buns eaten by some student to be minimum.</p><p>Help the teacher, get the maximum number of buns that some pupils will have to eat to achieve the goal of the teacher. Also, get one of the possible ways for achieving the objective, namely, the height of the lowest student in the end and the step of the resulting progression.</p></div><div class="input-specification"><p>The single line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup></span>) — the number of students. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers — the heights of all students. The height of one student is an integer which absolute value doesn't exceed <span class="tex-span">10<sup class="upper-index">4</sup></span>.</p></div><div class="output-specification"><p>In the first line print the maximum number of buns eaten by some student to achieve the teacher's aim. In the second line, print two space-separated integers — the height of the lowest student in the end and the step of the progression. Please, pay attention that the step should be non-negative.</p><p>If there are multiple possible answers, you can print any of them.</p></div>

## Input

<p>The single line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup></span>) — the number of students. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers — the heights of all students. The height of one student is an integer which absolute value doesn't exceed <span class="tex-span">10<sup class="upper-index">4</sup></span>.</p>

## Output

<p>In the first line print the maximum number of buns eaten by some student to achieve the teacher's aim. In the second line, print two space-separated integers — the height of the lowest student in the end and the step of the progression. Please, pay attention that the step should be non-negative.</p><p>If there are multiple possible answers, you can print any of them.</p>





```input1
5
-3 -4 -2 -3 3

```




```input2
5
2 -3 -1 -4 3

```




```output1
2
-3 1

```




```output2
1
-4 2

```



## Note

<p>Lets look at the first sample. We can proceed in the following manner:</p><ul> <li> don't feed the 1-st student, his height will stay equal to -3; </li><li> give two buns of the first type to the 2-nd student, his height become equal to -2; </li><li> give two buns of the first type to the 3-rd student, his height become equal to 0; </li><li> give two buns of the first type to the 4-th student, his height become equal to -1; </li><li> give two buns of the second type to the 5-th student, his height become equal to 1. </li></ul><p>To sum it up, when the students line up in non-decreasing height it will be an arithmetic progression: -3, -2, -1, 0, 1. The height of the lowest student is equal to -3, the step of the progression is equal to 1. The maximum number of buns eaten by one student is equal to 2.</p>
