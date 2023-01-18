## Description

<div><p>Emuskald is addicted to Codeforces, and keeps refreshing the main page not to miss any changes in the "recent actions" list. He likes to read thread conversations where each thread consists of multiple messages.</p><p>Recent actions shows a list of <span class="tex-span"><i>n</i></span> different threads ordered by the time of the latest message in the thread. When a new message is posted in a thread that thread jumps on the top of the list. No two messages of different threads are ever posted at the same time.</p><p>Emuskald has just finished reading all his opened threads and refreshes the main page for some more messages to feed his addiction. He notices that no new threads have appeared in the list and at the <span class="tex-span"><i>i</i></span>-th place in the list there is a thread that was at the <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>-th place before the refresh. He doesn't want to waste any time reading old messages so he wants to open only threads with new messages.</p><p>Help Emuskald find out the number of threads that <span class="tex-font-style-bf">surely</span> have new messages. A thread <span class="tex-span"><i>x</i></span> surely has a new message if there is no such sequence of thread updates (posting messages) that both conditions hold: </p><ol> <li> thread <span class="tex-span"><i>x</i></span> is not updated (it has no new messages); </li><li> the list order 1, 2, ..., <span class="tex-span"><i>n</i></span> changes to <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span>. </li></ol></div><div class="input-specification"><p>The first line of input contains an integer <span class="tex-span"><i>n</i></span>, the number of threads (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The next line contains a list of <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) is the old position of the <span class="tex-span"><i>i</i></span>-th thread in the new list. It is guaranteed that all of the <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p></div><div class="output-specification"><p>Output a single integer — the number of threads that surely contain a new message.</p></div>

## Input

<p>The first line of input contains an integer <span class="tex-span"><i>n</i></span>, the number of threads (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The next line contains a list of <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) is the old position of the <span class="tex-span"><i>i</i></span>-th thread in the new list. It is guaranteed that all of the <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p>

## Output

<p>Output a single integer — the number of threads that surely contain a new message.</p>





```input1
5
5 2 1 3 4

```




```input2
3
1 2 3

```




```input3
4
4 3 2 1

```




```output1
2

```




```output2
0

```




```output3
3

```



## Note

<p>In the first test case, threads 2 and 5 are placed before the thread 1, so these threads must contain new messages. Threads 1, 3 and 4 may contain no new messages, if only threads 2 and 5 have new messages.</p><p>In the second test case, there may be no new messages at all, since the thread order hasn't changed.</p><p>In the third test case, only thread 1 can contain no new messages.</p>
