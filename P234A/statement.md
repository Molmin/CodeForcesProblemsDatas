## Description

<div><p>One fine October day a mathematics teacher Vasily Petrov went to a class and saw there <span class="tex-span"><i>n</i></span> pupils who sat at the <img align="middle" class="tex-formula" src="file://8YTZXEU0.png" style="max-width: 100.0%;max-height: 100.0%;"> desks, two people at each desk. Vasily quickly realized that number <span class="tex-span"><i>n</i></span> is even. Like all true mathematicians, Vasily has all students numbered from 1 to <span class="tex-span"><i>n</i></span>.</p><p>But Vasily Petrov did not like the way the children were seated at the desks. According to him, the students whose numbers differ by <span class="tex-span">1</span>, can not sit together, as they talk to each other all the time, distract others and misbehave.</p><p>On the other hand, if a righthanded student sits at the left end of the desk and a lefthanded student sits at the right end of the desk, they hit elbows all the time and distract each other. In other cases, the students who sit at the same desk, do not interfere with each other.</p><p>Vasily knows very well which students are lefthanders and which ones are righthanders, and he asks you to come up with any order that meets these two uncomplicated conditions (students do not talk to each other and do not bump their elbows). It is guaranteed that the input is such that at least one way to seat the students always exists.</p></div><div class="input-specification"><p>The first input line contains a single even integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">4 ≤ <i>n</i> ≤ 100</span>) — the number of students in the class. The second line contains exactly <span class="tex-span"><i>n</i></span> capital English letters "L" and "R". If the <span class="tex-span"><i>i</i></span>-th letter at the second line equals "L", then the student number <span class="tex-span"><i>i</i></span> is a lefthander, otherwise he is a righthander.</p></div><div class="output-specification"><p>Print <img align="middle" class="tex-formula" src="file://yJhYC8b0.png" style="max-width: 100.0%;max-height: 100.0%;"> integer pairs, one pair per line. In the <span class="tex-span"><i>i</i></span>-th line print the numbers of students that will sit at the <span class="tex-span"><i>i</i></span>-th desk. The first number in the pair stands for the student who is sitting to the left, and the second number stands for the student who is sitting to the right. Separate the numbers in the pairs by spaces. If there are multiple solutions, print any of them.</p></div>

## Input

<p>The first input line contains a single even integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">4 ≤ <i>n</i> ≤ 100</span>) — the number of students in the class. The second line contains exactly <span class="tex-span"><i>n</i></span> capital English letters "L" and "R". If the <span class="tex-span"><i>i</i></span>-th letter at the second line equals "L", then the student number <span class="tex-span"><i>i</i></span> is a lefthander, otherwise he is a righthander.</p>

## Output

<p>Print <img align="middle" class="tex-formula" src="file://yJhYC8b0.png" style="max-width: 100.0%;max-height: 100.0%;"> integer pairs, one pair per line. In the <span class="tex-span"><i>i</i></span>-th line print the numbers of students that will sit at the <span class="tex-span"><i>i</i></span>-th desk. The first number in the pair stands for the student who is sitting to the left, and the second number stands for the student who is sitting to the right. Separate the numbers in the pairs by spaces. If there are multiple solutions, print any of them.</p>





```input1
6
LLRLLL

```




```input2
4
RRLL

```




```output1
1 4
2 5
6 3

```




```output2
3 1
4 2

```


