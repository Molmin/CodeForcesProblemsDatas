## Description

<div><p>Yura has a team of <span class="tex-span"><i>k</i></span> developers and a list of <span class="tex-span"><i>n</i></span> tasks numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Yura is going to choose some tasks to be done this week. Due to strange Looksery habits the numbers of chosen tasks should be a segment of consecutive integers containing <span class="tex-font-style-bf">no less than 2 numbers</span>, i. e. a sequence of form <span class="tex-span"><i>l</i>, <i>l</i> + 1, ..., <i>r</i></span> for some <span class="tex-span">1 ≤ <i>l</i> &lt; <i>r</i> ≤ <i>n</i></span>. </p><p>Every task <span class="tex-span"><i>i</i></span> has an integer number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> associated with it denoting how many man-hours are required to complete the <span class="tex-span"><i>i</i></span>-th task. Developers are not self-confident at all, and they are actually afraid of difficult tasks. Knowing that, Yura decided to pick up a hardest task (the one that takes the biggest number of man-hours to be completed, among several hardest tasks with same difficulty level he chooses arbitrary one) and complete it on his own. So, if tasks with numbers <span class="tex-span">[<i>l</i>, <i>r</i>]</span> are chosen then the developers are left with <span class="tex-span"><i>r</i> - <i>l</i></span> tasks to be done by themselves. </p><p>Every developer can spend any integer amount of hours over any task, but when they are done with the whole assignment there should be exactly <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> man-hours spent over the <span class="tex-span"><i>i</i></span>-th task. </p><p>The last, but not the least problem with developers is that one gets angry if he works more than another developer. A set of tasks <span class="tex-span">[<i>l</i>, <i>r</i>]</span> is considered <span class="tex-font-style-it">good</span> if it is possible to find such a distribution of work that allows to complete all the tasks and to have every developer working for the same amount of time (amount of work performed by Yura doesn't matter for other workers as well as for him).</p><p>For example, let's suppose that Yura have chosen tasks with following difficulties: <span class="tex-span"><i>a</i> = [1, 2, 3, 4]</span>, and he has three developers in his disposal. He takes the hardest fourth task to finish by himself, and the developers are left with tasks with difficulties <span class="tex-span">[1, 2, 3]</span>. If the first one spends an hour on the first task and an hour on the third one, the second developer spends two hours on the second task and the third developer spends two hours on the third task, then they are done, since every developer worked exactly for two hours and every task has been worked over for the required amount of time. As another example, if the first task required two hours instead of one to be completed then it would be impossible to assign the tasks in a way described above. </p><p>Besides work, Yura is fond of problem solving. He wonders how many pairs <span class="tex-span">(<i>l</i>, <i>r</i>)</span> (<span class="tex-span">1 ≤ <i>l</i> &lt; <i>r</i> ≤ <i>n</i></span>) exists such that a segment <span class="tex-span">[<i>l</i>, <i>r</i>]</span> is <span class="tex-font-style-it">good</span>? Yura has already solved this problem, but he has no time to write the code. Please, help Yura and implement the solution for this problem. </p></div><div class="input-specification"><p>The first line of input contains two positive integers: <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 300 000, 1 ≤ <i>k</i> ≤ 1 000 000)</span>, the number of tasks in the list and the number of developers in Yura's disposal. </p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). </p></div><div class="output-specification"><p>Output a single integer — the number of pairs <span class="tex-span">(<i>l</i>, <i>r</i>)</span> satisfying the conditions from the statement.</p></div>

## Input

<p>The first line of input contains two positive integers: <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 300 000, 1 ≤ <i>k</i> ≤ 1 000 000)</span>, the number of tasks in the list and the number of developers in Yura's disposal. </p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). </p>

## Output

<p>Output a single integer — the number of pairs <span class="tex-span">(<i>l</i>, <i>r</i>)</span> satisfying the conditions from the statement.</p>





```input1
4 3
1 2 3 4

```




```input2
4 2
4 4 7 4

```




```output1
3

```




```output2
6

```



## Note

<p>In the first sample there are three good segments:</p><ol><li> <span class="tex-span">[1;3]</span> — the hardest task requires <span class="tex-span">3</span> man-hours, so there are tasks left that require <span class="tex-span">1</span> and <span class="tex-span">2</span> man-hours. A solution is to make first developer work on the first task for an hour, while second and third developers work on the second task. Each developer works exactly one hour.</li><li> <span class="tex-span">[1;4]</span> — the hardest task requires <span class="tex-span">4</span> man-hours, so there are tasks left that require <span class="tex-span">1</span>, <span class="tex-span">2</span> and <span class="tex-span">3</span> man-hours. If the first developer spends an hour on the first task and an hour on the third one, the second developer spends two hours on the second task and the third developer spends two hours on the third task, then they are done, since every developer worked exactly for two hours.</li><li> <span class="tex-span">[3;4]</span> — the hardest task requires <span class="tex-span">4</span> man-hours, so there is only one task left that requires <span class="tex-span">3</span> man-hours. A solution is to make each developer work for an hour.</li></ol>
