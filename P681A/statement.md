## Description

<div><p>Codeforces user' handle color depends on his rating&nbsp;— it is red if his rating is greater or equal to <span class="tex-span">2400</span>; it is orange if his rating is less than <span class="tex-span">2400</span> but greater or equal to <span class="tex-span">2200</span>, etc. Each time participant takes part in a rated contest, his rating is changed depending on his performance.</p><p>Anton wants the color of his handle to become red. He considers his performance in the rated contest to be <span class="tex-font-style-it">good</span> if he outscored some participant, whose handle was colored red before the contest and his rating has increased after it.</p><p>Anton has written a program that analyses contest results and determines whether he performed good or not. Are you able to do the same?</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of participants Anton has outscored in this contest .</p><p>The next <span class="tex-span"><i>n</i></span> lines describe participants results: the <span class="tex-span"><i>i</i></span>-th of them consists of a participant handle <span class="tex-span"><i>name</i><sub class="lower-index"><i>i</i></sub></span> and two integers <span class="tex-span"><i>before</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>after</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 4000 ≤ <i>before</i><sub class="lower-index"><i>i</i></sub>, <i>after</i><sub class="lower-index"><i>i</i></sub> ≤ 4000</span>)&nbsp;— participant's rating before and after the contest, respectively. Each handle is a non-empty string, consisting of no more than <span class="tex-span">10</span> characters, which might be lowercase and uppercase English letters, digits, characters «<span class="tex-font-style-tt">_</span>» and «<span class="tex-font-style-tt">-</span>» characters.</p><p>It is guaranteed that all handles are distinct.</p></div><div class="output-specification"><p>Print «<span class="tex-font-style-tt">YES</span>» (quotes for clarity), if Anton has performed good in the contest and «<span class="tex-font-style-tt">NO</span>» (quotes for clarity) otherwise.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of participants Anton has outscored in this contest .</p><p>The next <span class="tex-span"><i>n</i></span> lines describe participants results: the <span class="tex-span"><i>i</i></span>-th of them consists of a participant handle <span class="tex-span"><i>name</i><sub class="lower-index"><i>i</i></sub></span> and two integers <span class="tex-span"><i>before</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>after</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 4000 ≤ <i>before</i><sub class="lower-index"><i>i</i></sub>, <i>after</i><sub class="lower-index"><i>i</i></sub> ≤ 4000</span>)&nbsp;— participant's rating before and after the contest, respectively. Each handle is a non-empty string, consisting of no more than <span class="tex-span">10</span> characters, which might be lowercase and uppercase English letters, digits, characters «<span class="tex-font-style-tt">_</span>» and «<span class="tex-font-style-tt">-</span>» characters.</p><p>It is guaranteed that all handles are distinct.</p>

## Output

<p>Print «<span class="tex-font-style-tt">YES</span>» (quotes for clarity), if Anton has performed good in the contest and «<span class="tex-font-style-tt">NO</span>» (quotes for clarity) otherwise.</p>





```input1
3
Burunduk1 2526 2537
BudAlNik 2084 2214
subscriber 2833 2749

```




```input2
3
Applejack 2400 2400
Fluttershy 2390 2431
Pinkie_Pie -2500 -2450

```




```output1
YES
```




```output2
NO
```



## Note

<p>In the first sample, Anton has outscored user with handle <span class="tex-font-style-tt">Burunduk1</span>, whose handle was colored red before the contest and his rating has increased after the contest.</p><p>In the second sample, <span class="tex-font-style-tt">Applejack</span>'s rating has not increased after the contest, while both <span class="tex-font-style-tt">Fluttershy</span>'s and <span class="tex-font-style-tt">Pinkie_Pie</span>'s handles were not colored red before the contest.</p>
