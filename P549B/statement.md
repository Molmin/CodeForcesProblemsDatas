## Description

<div><p>The Looksery company, consisting of <span class="tex-span"><i>n</i></span> staff members, is planning another big party. Every employee has his phone number and the phone numbers of his friends in the phone book. Everyone who comes to the party, sends messages to his contacts about how cool it is. At the same time everyone is trying to spend as much time on the fun as possible, so they send messages to everyone without special thinking, moreover, each person even sends a message <span class="tex-font-style-bf">to himself or herself</span>.</p><p>Igor and Max, Looksery developers, started a dispute on how many messages each person gets. Igor indicates <span class="tex-span"><i>n</i></span> numbers, the <span class="tex-span"><i>i</i></span>-th of which indicates how many messages, in his view, the <span class="tex-span"><i>i</i></span>-th employee is going to take. If Igor guesses correctly at least one of these numbers, he wins, otherwise Max wins.</p><p>You support Max in this debate, so you need, given the contact lists of the employees, to determine whether there is a situation where Igor loses. Specifically, you need to determine which employees should come to the party, and which should not, so after all the visitors send messages to their contacts, each employee received a number of messages that is different from what Igor stated.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of employees of company Looksery.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain the description of the contact lists of the employees. The <span class="tex-span"><i>i</i></span>-th of these lines contains a string of length <span class="tex-span"><i>n</i></span>, consisting of digits zero and one, specifying the contact list of the <span class="tex-span"><i>i</i></span>-th employee. If the <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th string equals <span class="tex-font-style-tt">1</span>, then the <span class="tex-span"><i>j</i></span>-th employee is in the <span class="tex-span"><i>i</i></span>-th employee's contact list, otherwise he isn't. It is guaranteed that the <span class="tex-span"><i>i</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th line is always equal to <span class="tex-font-style-tt">1</span>.</p><p>The last line contains <span class="tex-span"><i>n</i></span> space-separated integers: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> represents the number of messages that the <span class="tex-span"><i>i</i></span>-th employee should get according to Igor.</p></div><div class="output-specification"><p>In the first line print a single integer <span class="tex-span"><i>m</i></span> — the number of employees who should come to the party so that Igor loses the dispute.</p><p>In the second line print <span class="tex-span"><i>m</i></span> space-separated integers — the numbers of these employees in an arbitrary order.</p><p>If Igor wins the dispute in any case, print <span class="tex-font-style-tt">-1</span>.</p><p>If there are multiple possible solutions, print any of them.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of employees of company Looksery.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain the description of the contact lists of the employees. The <span class="tex-span"><i>i</i></span>-th of these lines contains a string of length <span class="tex-span"><i>n</i></span>, consisting of digits zero and one, specifying the contact list of the <span class="tex-span"><i>i</i></span>-th employee. If the <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th string equals <span class="tex-font-style-tt">1</span>, then the <span class="tex-span"><i>j</i></span>-th employee is in the <span class="tex-span"><i>i</i></span>-th employee's contact list, otherwise he isn't. It is guaranteed that the <span class="tex-span"><i>i</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th line is always equal to <span class="tex-font-style-tt">1</span>.</p><p>The last line contains <span class="tex-span"><i>n</i></span> space-separated integers: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> represents the number of messages that the <span class="tex-span"><i>i</i></span>-th employee should get according to Igor.</p>

## Output

<p>In the first line print a single integer <span class="tex-span"><i>m</i></span> — the number of employees who should come to the party so that Igor loses the dispute.</p><p>In the second line print <span class="tex-span"><i>m</i></span> space-separated integers — the numbers of these employees in an arbitrary order.</p><p>If Igor wins the dispute in any case, print <span class="tex-font-style-tt">-1</span>.</p><p>If there are multiple possible solutions, print any of them.</p>





```input1
3
101
010
001
0 1 2

```




```input2
1
1
1

```




```input3
4
1111
0101
1110
0001
1 0 1 0

```




```output1
1
1 

```




```output2
0


```




```output3
4
1 2 3 4 

```



## Note

<p>In the first sample Igor supposes that the first employee will receive <span class="tex-span">0</span> messages. Since he isn't contained in any other contact list he must come to the party in order to receive one message from himself. If he is the only who come to the party then he will receive <span class="tex-span">1</span> message, the second employee will receive <span class="tex-span">0</span> messages and the third will also receive <span class="tex-span">1</span> message. Thereby Igor won't guess any number.</p><p>In the second sample if the single employee comes to the party he receives <span class="tex-span">1</span> message and Igor wins, so he shouldn't do it.</p><p>In the third sample the first employee will receive <span class="tex-span">2</span> messages, the second — <span class="tex-span">3</span>, the third — <span class="tex-span">2</span>, the fourth — <span class="tex-span">3</span>.</p>
