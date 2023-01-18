## Description

<div><p>Recently Pashmak has been employed in a transportation company. The company has <span class="tex-span"><i>k</i></span> buses and has a contract with a school which has <span class="tex-span"><i>n</i></span> students. The school planned to take the students to <span class="tex-span"><i>d</i></span> different places for <span class="tex-span"><i>d</i></span> days (each day in one place). Each day the company provides all the buses for the trip. Pashmak has to arrange the students in the buses. He wants to arrange the students in a way that no two students become close friends. In his ridiculous idea, two students will become close friends if and only if they are in the same buses for all <span class="tex-span"><i>d</i></span> days.</p><p>Please help Pashmak with his weird idea. Assume that each bus has an unlimited capacity.</p></div><div class="input-specification"><p>The first line of input contains three space-separated integers <span class="tex-span"><i>n</i>, <i>k</i>, <i>d</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>d</i> ≤ 1000;&nbsp;1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup>)</span>.</p></div><div class="output-specification"><p>If there is no valid arrangement just print <span class="tex-font-style-tt">-1</span>. Otherwise print <span class="tex-span"><i>d</i></span> lines, in each of them print <span class="tex-span"><i>n</i></span> integers. The <span class="tex-span"><i>j</i></span>-th integer of the <span class="tex-span"><i>i</i></span>-th line shows which bus the <span class="tex-span"><i>j</i></span>-th student has to take on the <span class="tex-span"><i>i</i></span>-th day. You can assume that the buses are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i></span>.</p></div>

## Input

<p>The first line of input contains three space-separated integers <span class="tex-span"><i>n</i>, <i>k</i>, <i>d</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>d</i> ≤ 1000;&nbsp;1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup>)</span>.</p>

## Output

<p>If there is no valid arrangement just print <span class="tex-font-style-tt">-1</span>. Otherwise print <span class="tex-span"><i>d</i></span> lines, in each of them print <span class="tex-span"><i>n</i></span> integers. The <span class="tex-span"><i>j</i></span>-th integer of the <span class="tex-span"><i>i</i></span>-th line shows which bus the <span class="tex-span"><i>j</i></span>-th student has to take on the <span class="tex-span"><i>i</i></span>-th day. You can assume that the buses are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i></span>.</p>





```input1
3 2 2

```




```input2
3 2 1

```




```output1
1 1 2 
1 2 1 

```




```output2
-1

```



## Note

<p>Note that two students become close friends only if they share a bus each day. But the bus they share can differ from day to day.</p>
