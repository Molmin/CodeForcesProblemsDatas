## Description

<div><p>It's time polar bears Menshykov and Uslada from the zoo of St. Petersburg and elephant Horace from the zoo of Kiev got down to business. In total, there are <span class="tex-span"><i>n</i></span> tasks for the day and each animal should do each of these tasks. For each task, they have evaluated its difficulty. Also animals decided to do the tasks in order of their difficulty. Unfortunately, some tasks can have the same difficulty, so the order in which one can perform the tasks may vary.</p><p>Menshykov, Uslada and Horace ask you to deal with this nuisance and come up with individual plans for each of them. The plan is a sequence describing the order in which an animal should do all the <span class="tex-span"><i>n</i></span> tasks. Besides, each of them wants to have its own unique plan. Therefore three plans must form three different sequences. You are to find the required plans, or otherwise deliver the sad news to them by stating that it is impossible to come up with three distinct plans for the given tasks.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>) — the number of tasks. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>h</i><sub class="lower-index">1</sub>, <i>h</i><sub class="lower-index">2</sub>, ..., <i>h</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 2000</span>), where <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> is the difficulty of the <span class="tex-span"><i>i</i></span>-th task. The larger number <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> is, the more difficult the <span class="tex-span"><i>i</i></span>-th task is.</p></div><div class="output-specification"><p>In the first line print "<span class="tex-font-style-tt">YES</span>" (without the quotes), if it is possible to come up with three distinct plans of doing the tasks. Otherwise print in the first line "<span class="tex-font-style-tt">NO</span>" (without the quotes). If three desired plans do exist, print in the second line <span class="tex-span"><i>n</i></span> distinct integers that represent the numbers of the tasks in the order they are done according to the first plan. In the third and fourth line print two remaining plans in the same form.</p><p>If there are multiple possible answers, you can print any of them.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>) — the number of tasks. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>h</i><sub class="lower-index">1</sub>, <i>h</i><sub class="lower-index">2</sub>, ..., <i>h</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 2000</span>), where <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> is the difficulty of the <span class="tex-span"><i>i</i></span>-th task. The larger number <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> is, the more difficult the <span class="tex-span"><i>i</i></span>-th task is.</p>

## Output

<p>In the first line print "<span class="tex-font-style-tt">YES</span>" (without the quotes), if it is possible to come up with three distinct plans of doing the tasks. Otherwise print in the first line "<span class="tex-font-style-tt">NO</span>" (without the quotes). If three desired plans do exist, print in the second line <span class="tex-span"><i>n</i></span> distinct integers that represent the numbers of the tasks in the order they are done according to the first plan. In the third and fourth line print two remaining plans in the same form.</p><p>If there are multiple possible answers, you can print any of them.</p>





```input1
4
1 3 3 1

```




```input2
5
2 4 1 4 8

```




```output1
YES
1 4 2 3 
4 1 2 3 
4 1 3 2 

```




```output2
NO
```



## Note

<p>In the first sample the difficulty of the tasks sets one limit: tasks 1 and 4 must be done before tasks 2 and 3. That gives the total of four possible sequences of doing tasks : [1, 4, 2, 3], [4, 1, 2, 3], [1, 4, 3, 2], [4, 1, 3, 2]. You can print any three of them in the answer.</p><p>In the second sample there are only two sequences of tasks that meet the conditions — [3, 1, 2, 4, 5] and [3, 1, 4, 2, 5]. Consequently, it is impossible to make three distinct sequences of tasks.</p>
