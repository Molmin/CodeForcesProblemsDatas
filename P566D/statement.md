## Description

<div><p>Even the most successful company can go through a crisis period when you have to make a hard decision — to restructure, discard and merge departments, fire employees and do other unpleasant stuff. Let's consider the following model of a company.</p><p>There are <span class="tex-span"><i>n</i></span> people working for the Large Software Company. Each person belongs to some <span class="tex-font-style-it">department</span>. Initially, each person works on his own project in his own department (thus, each company initially consists of <span class="tex-span"><i>n</i></span> departments, one person in each).</p><p>However, harsh times have come to the company and the management had to hire a crisis manager who would rebuild the working process in order to boost efficiency. Let's use <span class="tex-span"><i>team</i>(<i>person</i>)</span> to represent a team where person <span class="tex-span"><i>person</i></span> works. A crisis manager can make decisions of two types:</p><ol> <li> Merge departments <span class="tex-span"><i>team</i>(<i>x</i>)</span> and <span class="tex-span"><i>team</i>(<i>y</i>)</span> into one large department containing all the employees of <span class="tex-span"><i>team</i>(<i>x</i>)</span> and <span class="tex-span"><i>team</i>(<i>y</i>)</span>, where <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i></span>) — are numbers of two of some company employees. If <span class="tex-span"><i>team</i>(<i>x</i>)</span> matches <span class="tex-span"><i>team</i>(<i>y</i>)</span>, then nothing happens. </li><li> Merge departments <span class="tex-span"><i>team</i>(<i>x</i>), <i>team</i>(<i>x</i> + 1), ..., <i>team</i>(<i>y</i>)</span>, where <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>y</i> ≤ <i>n</i></span>) — the numbers of some two employees of the company. </li></ol><p>At that the crisis manager can sometimes wonder whether employees <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i></span>) work at the same department.</p><p>Help the crisis manager and answer all of his queries.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 500 000</span>) — the number of the employees of the company and the number of queries the crisis manager has.</p><p>Next <span class="tex-span"><i>q</i></span> lines contain the queries of the crisis manager. Each query looks like <span class="tex-span"><i>type</i>&nbsp;<i>x</i>&nbsp;<i>y</i></span>, where <img align="middle" class="tex-formula" src="file://sWkn2Ht1.png" style="max-width: 100.0%;max-height: 100.0%;">. If <span class="tex-span"><i>type</i> = 1</span> or <span class="tex-span"><i>type</i> = 2</span>, then the query represents the decision of a crisis manager about merging departments of the first and second types respectively. If <span class="tex-span"><i>type</i> = 3</span>, then your task is to determine whether employees <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> work at the same department. Note that <span class="tex-span"><i>x</i></span> can be equal to <span class="tex-span"><i>y</i></span> in the query of any type.</p></div><div class="output-specification"><p>For each question of type <span class="tex-span">3</span> print "<span class="tex-font-style-tt">YES</span>" or "<span class="tex-font-style-tt">NO</span>" (without the quotes), depending on whether the corresponding people work in the same department.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 500 000</span>) — the number of the employees of the company and the number of queries the crisis manager has.</p><p>Next <span class="tex-span"><i>q</i></span> lines contain the queries of the crisis manager. Each query looks like <span class="tex-span"><i>type</i>&nbsp;<i>x</i>&nbsp;<i>y</i></span>, where <img align="middle" class="tex-formula" src="file://sWkn2Ht1.png" style="max-width: 100.0%;max-height: 100.0%;">. If <span class="tex-span"><i>type</i> = 1</span> or <span class="tex-span"><i>type</i> = 2</span>, then the query represents the decision of a crisis manager about merging departments of the first and second types respectively. If <span class="tex-span"><i>type</i> = 3</span>, then your task is to determine whether employees <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> work at the same department. Note that <span class="tex-span"><i>x</i></span> can be equal to <span class="tex-span"><i>y</i></span> in the query of any type.</p>

## Output

<p>For each question of type <span class="tex-span">3</span> print "<span class="tex-font-style-tt">YES</span>" or "<span class="tex-font-style-tt">NO</span>" (without the quotes), depending on whether the corresponding people work in the same department.</p>





```input1
8 6
3 2 5
1 2 5
3 2 5
2 4 7
2 1 2
3 1 7

```




```output1
NO
YES
YES

```


