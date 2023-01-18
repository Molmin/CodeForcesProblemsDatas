## Description

<div><p>Some large corporation where Polycarpus works has its own short message service center (SMSC). The center's task is to send all sorts of crucial information. Polycarpus decided to check the efficiency of the SMSC. </p><p>For that, he asked to give him the statistics of the performance of the SMSC for some period of time. In the end, Polycarpus got a list of <span class="tex-span"><i>n</i></span> tasks that went to the SMSC of the corporation. Each task was described by the time it was received by the SMSC and the number of text messages to send. More formally, the <span class="tex-span"><i>i</i></span>-th task was described by two integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> — the receiving time (the second) and the number of the text messages, correspondingly.</p><p>Polycarpus knows that the SMSC cannot send more than one text message per second. The SMSC uses a queue to organize its work. Consider a time moment <span class="tex-span"><i>x</i></span>, the SMSC work at that moment as follows:</p><ol> <li> If at the time moment <span class="tex-span"><i>x</i></span> the queue is not empty, then SMSC sends one message from the queue (SMSC gets the message from the head of the queue). Otherwise it doesn't send messages at the time moment <span class="tex-span"><i>x</i></span>. </li><li> If at the time moment <span class="tex-span"><i>x</i></span> SMSC receives a task, then it adds to the queue all the messages from this task (SMSC adds messages to the tail of the queue). Note, that the messages from the task cannot be send at time moment <span class="tex-span"><i>x</i></span>. That's because the decision about sending message or not is made at point 1 before adding these messages to the queue. </li></ol><p>Given the information about all <span class="tex-span"><i>n</i></span> tasks, Polycarpus wants to count two values: the time when the last text message was sent and the maximum size of the queue at some time. Help him count these two characteristics he needs to evaluate the efficiency of the SMSC.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup>)</span> — the number of tasks of the SMSC. Next <span class="tex-span"><i>n</i></span> lines contain the tasks' descriptions: the <span class="tex-span"><i>i</i></span>-th line contains two space-separated integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span> — the time (the second) when the <span class="tex-span"><i>i</i></span>-th task was received and the number of messages to send, correspondingly.</p><p>It is guaranteed that all tasks were received at different moments of time. It is guaranteed that the tasks are sorted in the chronological order, that is, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> &lt; <i>t</i><sub class="lower-index"><i>i</i> + 1</sub></span> for all integer <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> &lt; <i>n</i>)</span>.</p></div><div class="output-specification"><p>In a single line print two space-separated integers — the time when the last text message was sent and the maximum queue size at a certain moment of time.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup>)</span> — the number of tasks of the SMSC. Next <span class="tex-span"><i>n</i></span> lines contain the tasks' descriptions: the <span class="tex-span"><i>i</i></span>-th line contains two space-separated integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span> — the time (the second) when the <span class="tex-span"><i>i</i></span>-th task was received and the number of messages to send, correspondingly.</p><p>It is guaranteed that all tasks were received at different moments of time. It is guaranteed that the tasks are sorted in the chronological order, that is, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> &lt; <i>t</i><sub class="lower-index"><i>i</i> + 1</sub></span> for all integer <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> &lt; <i>n</i>)</span>.</p>

## Output

<p>In a single line print two space-separated integers — the time when the last text message was sent and the maximum queue size at a certain moment of time.</p>





```input1
2
1 1
2 1

```




```input2
1
1000000 10

```




```input3
3
3 3
4 3
5 3

```




```output1
3 1

```




```output2
1000010 10

```




```output3
12 7

```



## Note

<p>In the first test sample: </p><ul> <li> second 1: the first message has appeared in the queue, the queue's size is 1; </li><li> second 2: the first message is sent, the second message has been received, the queue's size is 1; </li><li> second 3: the second message is sent, the queue's size is 0, </li></ul><p>Thus, the maximum size of the queue is 1, the last message was sent at the second 3.</p>
