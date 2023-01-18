## Description

<div><p>While most students still sit their exams, the tractor college has completed the summer exam session. In fact, students study only one subject at this college — the Art of Operating a Tractor. Therefore, at the end of a term a student gets only one mark, a three (satisfactory), a four (good) or a five (excellent). Those who score lower marks are unfortunately expelled.</p><p>The college has <span class="tex-span"><i>n</i></span> students, and oddly enough, each of them can be on scholarship. The size of the scholarships varies each term. Since the end-of-the-term exam has just ended, it's time to determine the size of the scholarship to the end of next term.</p><p>The monthly budget for the scholarships of the Tractor college is <span class="tex-span"><i>s</i></span> rubles. To distribute the budget optimally, you must follow these rules:</p><ul> <li> The students who received the same mark for the exam, should receive the same scholarship;</li><li> Let us denote the size of the scholarship (in roubles) for students who have received marks <span class="tex-span">3</span>, <span class="tex-span">4</span> and <span class="tex-span">5</span> for the exam, as <span class="tex-span"><i>k</i><sub class="lower-index">3</sub></span>, <span class="tex-span"><i>k</i><sub class="lower-index">4</sub></span> and <span class="tex-span"><i>k</i><sub class="lower-index">5</sub></span>, respectively. The values <span class="tex-span"><i>k</i><sub class="lower-index">3</sub></span>, <span class="tex-span"><i>k</i><sub class="lower-index">4</sub></span> and <span class="tex-span"><i>k</i><sub class="lower-index">5</sub></span> must be integers and satisfy the inequalities <span class="tex-span">0 ≤ <i>k</i><sub class="lower-index">3</sub> ≤ <i>k</i><sub class="lower-index">4</sub> ≤ <i>k</i><sub class="lower-index">5</sub></span>;</li><li> Let's assume that <span class="tex-span"><i>c</i><sub class="lower-index">3</sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index">4</sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index">5</sub></span> show how many students received marks <span class="tex-span">3</span>, <span class="tex-span">4</span> and <span class="tex-span">5</span> for the exam, respectively. The budget of the scholarship should be fully spent on them, that is, <span class="tex-span"><i>c</i><sub class="lower-index">3</sub>·<i>k</i><sub class="lower-index">3</sub> + <i>c</i><sub class="lower-index">4</sub>·<i>k</i><sub class="lower-index">4</sub> + <i>c</i><sub class="lower-index">5</sub>·<i>k</i><sub class="lower-index">5</sub> = <i>s</i></span>;</li><li> Let's introduce function <img align="middle" class="tex-formula" src="file://ewOaE6I1.png" style="max-width: 100.0%;max-height: 100.0%;"> — the value that shows how well the scholarships are distributed between students. In the optimal distribution function <span class="tex-span"><i>f</i>(<i>k</i><sub class="lower-index">3</sub>, <i>k</i><sub class="lower-index">4</sub>, <i>k</i><sub class="lower-index">5</sub>)</span> takes the <span class="tex-font-style-bf">minimum</span> possible value. </li></ul><p>Given the results of the exam, and the budget size <span class="tex-span"><i>s</i></span>, you have to find the optimal distribution of the scholarship.</p></div><div class="input-specification"><p>The first line has two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>s</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 300, 1 ≤ <i>s</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the number of students and the budget size for the scholarship, respectively. The second line contains <span class="tex-span"><i>n</i></span> integers, where the <span class="tex-span"><i>i</i></span>-th number represents the mark that the <span class="tex-span"><i>i</i></span>-th student got for the exam. It is guaranteed that at each mark was given to at least one student.</p></div><div class="output-specification"><p>On a single line print three integers <span class="tex-span"><i>k</i><sub class="lower-index">3</sub></span>, <span class="tex-span"><i>k</i><sub class="lower-index">4</sub></span> and <span class="tex-span"><i>k</i><sub class="lower-index">5</sub></span> — the sought values that represent the optimal distribution of the scholarships. If there are multiple optimal answers, print any of them. If there is no answer, print -1.</p></div>

## Input

<p>The first line has two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>s</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 300, 1 ≤ <i>s</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the number of students and the budget size for the scholarship, respectively. The second line contains <span class="tex-span"><i>n</i></span> integers, where the <span class="tex-span"><i>i</i></span>-th number represents the mark that the <span class="tex-span"><i>i</i></span>-th student got for the exam. It is guaranteed that at each mark was given to at least one student.</p>

## Output

<p>On a single line print three integers <span class="tex-span"><i>k</i><sub class="lower-index">3</sub></span>, <span class="tex-span"><i>k</i><sub class="lower-index">4</sub></span> and <span class="tex-span"><i>k</i><sub class="lower-index">5</sub></span> — the sought values that represent the optimal distribution of the scholarships. If there are multiple optimal answers, print any of them. If there is no answer, print -1.</p>





```input1
5 11
3 4 3 5 5

```




```input2
6 15
5 3 3 4 4 5

```




```output1
1 3 3

```




```output2
-1

```


