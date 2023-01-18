## Description

<div><p>As a German University in Cairo (GUC) student and a basketball player, Herr Wafa was delighted once he heard the news. GUC is finally participating in the Annual Basketball Competition (ABC). </p><p>A team is to be formed of <span class="tex-span"><i>n</i></span> players, all of which are GUC students. However, the team might have players belonging to different departments. There are <span class="tex-span"><i>m</i></span> departments in GUC, numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>. Herr Wafa's department has number <span class="tex-span"><i>h</i></span>. For each department <span class="tex-span"><i>i</i></span>, Herr Wafa knows number <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> — how many students who play basketball belong to this department.</p><p>Herr Wafa was also able to guarantee a spot on the team, using his special powers. But since he hates floating-point numbers, he needs your help at finding the probability that he will have at least one teammate belonging to his department. </p><p>Note that every possible team containing Herr Wafa is equally probable. Consider all the students different from each other.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>h</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100, 1 ≤ <i>m</i> ≤ 1000, 1 ≤ <i>h</i> ≤ <i>m</i></span>) — the number of players on the team, the number of departments in GUC and Herr Wafa's department, correspondingly. </p><p>The second line contains a single-space-separated list of <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), denoting the number of students in the <span class="tex-span"><i>i</i></span>-th department. Note that <span class="tex-span"><i>s</i><sub class="lower-index"><i>h</i></sub></span> includes Herr Wafa.</p></div><div class="output-specification"><p>Print the probability that Herr Wafa will have at least one teammate from his department. If there is not enough basketball players in GUC to participate in ABC, print -1. The answer will be accepted if it has absolute or relative error not exceeding <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>h</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100, 1 ≤ <i>m</i> ≤ 1000, 1 ≤ <i>h</i> ≤ <i>m</i></span>) — the number of players on the team, the number of departments in GUC and Herr Wafa's department, correspondingly. </p><p>The second line contains a single-space-separated list of <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), denoting the number of students in the <span class="tex-span"><i>i</i></span>-th department. Note that <span class="tex-span"><i>s</i><sub class="lower-index"><i>h</i></sub></span> includes Herr Wafa.</p>

## Output

<p>Print the probability that Herr Wafa will have at least one teammate from his department. If there is not enough basketball players in GUC to participate in ABC, print -1. The answer will be accepted if it has absolute or relative error not exceeding <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
3 2 1
2 1

```




```input2
3 2 1
1 1

```




```input3
3 2 1
2 2

```




```output1
1

```




```output2
-1

```




```output3
0.666667

```



## Note

<p>In the first example all 3 players (2 from department 1 and 1 from department 2) must be chosen for the team. Both players from Wafa's departments will be chosen, so he's guaranteed to have a teammate from his department.</p><p>In the second example, there are not enough players.</p><p>In the third example, there are three possibilities to compose the team containing Herr Wafa. In two of them the other player from Herr Wafa's department is part of the team.</p>
