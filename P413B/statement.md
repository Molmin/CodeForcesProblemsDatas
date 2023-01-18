## Description

<div><p>The R2 company has <span class="tex-span"><i>n</i></span> employees working for it. The work involves constant exchange of ideas, sharing the stories of success and upcoming challenging. For that, R2 uses a famous instant messaging program Spyke.</p><p>R2 has <span class="tex-span"><i>m</i></span> Spyke chats just to discuss all sorts of issues. In each chat, some group of employees exchanges messages daily. An employee can simultaneously talk in multiple chats. If some employee is in the <span class="tex-span"><i>k</i></span>-th chat, he can write messages to this chat and receive notifications about messages from this chat. If an employee writes a message in the chat, all other participants of the chat receive a message notification.</p><p>The R2 company is conducting an audit. Now the specialists study effective communication between the employees. For this purpose, they have a chat log and the description of chat structure. You, as one of audit specialists, are commissioned to write a program that will use this data to determine the total number of message notifications received by each employee.</p></div><div class="input-specification"><p>The first line contains three space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">4</sup>;&nbsp;1 ≤ <i>m</i> ≤ 10;&nbsp;1 ≤ <i>k</i> ≤ 2·10<sup class="upper-index">5</sup>)</span> — the number of the employees, the number of chats and the number of events in the log, correspondingly. </p><p>Next <span class="tex-span"><i>n</i></span> lines contain matrix <span class="tex-span"><i>a</i></span> of size <span class="tex-span"><i>n</i> × <i>m</i></span>, consisting of numbers zero and one. The element of this matrix, recorded in the <span class="tex-span"><i>j</i></span>-th column of the <span class="tex-span"><i>i</i></span>-th line, (let's denote it as <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span>) equals <span class="tex-span">1</span>, if the <span class="tex-span"><i>i</i></span>-th employee is the participant of the <span class="tex-span"><i>j</i></span>-th chat, otherwise the element equals <span class="tex-span">0</span>. Assume that the employees are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> and the chats are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>.</p><p>Next <span class="tex-span"><i>k</i></span> lines contain the description of the log events. The <span class="tex-span"><i>i</i></span>-th line contains two space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i>)</span> which mean that the employee number <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> sent one message to chat number <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>. It is guaranteed that employee number <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> is a participant of chat <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>. It is guaranteed that each chat contains at least two employees.</p></div><div class="output-specification"><p>Print in the single line <span class="tex-span"><i>n</i></span> space-separated integers, where the <span class="tex-span"><i>i</i></span>-th integer shows the number of message notifications the <span class="tex-span"><i>i</i></span>-th employee receives.</p></div>

## Input

<p>The first line contains three space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">4</sup>;&nbsp;1 ≤ <i>m</i> ≤ 10;&nbsp;1 ≤ <i>k</i> ≤ 2·10<sup class="upper-index">5</sup>)</span> — the number of the employees, the number of chats and the number of events in the log, correspondingly. </p><p>Next <span class="tex-span"><i>n</i></span> lines contain matrix <span class="tex-span"><i>a</i></span> of size <span class="tex-span"><i>n</i> × <i>m</i></span>, consisting of numbers zero and one. The element of this matrix, recorded in the <span class="tex-span"><i>j</i></span>-th column of the <span class="tex-span"><i>i</i></span>-th line, (let's denote it as <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span>) equals <span class="tex-span">1</span>, if the <span class="tex-span"><i>i</i></span>-th employee is the participant of the <span class="tex-span"><i>j</i></span>-th chat, otherwise the element equals <span class="tex-span">0</span>. Assume that the employees are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> and the chats are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>.</p><p>Next <span class="tex-span"><i>k</i></span> lines contain the description of the log events. The <span class="tex-span"><i>i</i></span>-th line contains two space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i>)</span> which mean that the employee number <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> sent one message to chat number <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>. It is guaranteed that employee number <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> is a participant of chat <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>. It is guaranteed that each chat contains at least two employees.</p>

## Output

<p>Print in the single line <span class="tex-span"><i>n</i></span> space-separated integers, where the <span class="tex-span"><i>i</i></span>-th integer shows the number of message notifications the <span class="tex-span"><i>i</i></span>-th employee receives.</p>





```input1
3 4 5
1 1 1 1
1 0 1 1
1 1 0 0
1 1
3 1
1 3
2 4
3 2

```




```input2
4 3 4
0 1 1
1 0 1
1 1 1
0 0 0
1 2
2 1
3 1
1 3

```




```output1
3 3 1
```




```output2
0 2 3 0
```


