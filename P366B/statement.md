## Description

<div><p>You helped Dima to have a great weekend, but it's time to work. Naturally, Dima, as all other men who have girlfriends, does everything wrong.</p><p>Inna and Dima are now in one room. Inna tells Dima off for everything he does in her presence. After Inna tells him off for something, she goes to another room, walks there in circles muttering about how useless her sweetheart is. During that time Dima has time to peacefully complete <span class="tex-span"><i>k</i> - 1</span> tasks. Then Inna returns and tells Dima off for the next task he does in her presence and goes to another room again. It continues until Dima is through with his tasks.</p><p>Overall, Dima has <span class="tex-span"><i>n</i></span> tasks to do, each task has a unique number from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Dima loves order, so he does tasks consecutively, starting from some task. For example, if Dima has <span class="tex-span">6</span> tasks to do in total, then, if he starts from the <span class="tex-span">5</span>-th task, the order is like that: first Dima does the <span class="tex-span">5</span>-th task, then the <span class="tex-span">6</span>-th one, then the <span class="tex-span">1</span>-st one, then the <span class="tex-span">2</span>-nd one, then the <span class="tex-span">3</span>-rd one, then the <span class="tex-span">4</span>-th one.</p><p>Inna tells Dima off (only lovingly and appropriately!) so often and systematically that he's very well learned the power with which she tells him off for each task. Help Dima choose the first task so that in total he gets told off with as little power as possible.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i>, <i>k</i>&nbsp;(1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>&nbsp;(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">3</sup>)</span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the power Inna tells Dima off with if she is present in the room while he is doing the <span class="tex-span"><i>i</i></span>-th task.</p><p>It is guaranteed that <span class="tex-span"><i>n</i></span> is divisible by <span class="tex-span"><i>k</i></span>.</p></div><div class="output-specification"><p>In a single line print the number of the task Dima should start with to get told off with as little power as possible. If there are multiple solutions, print the one with the minimum number of the first task to do.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i>, <i>k</i>&nbsp;(1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>&nbsp;(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">3</sup>)</span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the power Inna tells Dima off with if she is present in the room while he is doing the <span class="tex-span"><i>i</i></span>-th task.</p><p>It is guaranteed that <span class="tex-span"><i>n</i></span> is divisible by <span class="tex-span"><i>k</i></span>.</p>

## Output

<p>In a single line print the number of the task Dima should start with to get told off with as little power as possible. If there are multiple solutions, print the one with the minimum number of the first task to do.</p>





```input1
6 2
3 2 1 6 5 4

```




```input2
10 5
1 3 5 7 9 9 4 1 8 5

```




```output1
1

```




```output2
3

```



## Note

<p>Explanation of the first example.</p><p>If Dima starts from the first task, Inna tells him off with power 3, then Dima can do one more task (as <span class="tex-span"><i>k</i></span> = 2), then Inna tells him off for the third task with power 1, then she tells him off for the fifth task with power 5. Thus, Dima gets told off with total power 3 + 1 + 5 = 9. If Dima started from the second task, for example, then Inna would tell him off for tasks 2, 4 and 6 with power 2 + 6 + 4 = 12. </p><p>Explanation of the second example.</p><p>In the second example <span class="tex-span"><i>k</i></span> = 5, thus, Dima manages to complete 4 tasks in-between the telling off sessions. Thus, Inna tells Dima off for tasks number 1 and 6 (if he starts from 1 or 6), 2 and 7 (if he starts from 2 or 7) and so on. The optimal answer is to start from task 3 or 8, 3 has a smaller number, so the answer is 3.</p>
