## Description

<div><p>The Smart Beaver from ABBYY started cooperating with the Ministry of Defence. Now they train soldiers to move armoured columns. The training involves testing a new type of tanks that can transmit information. To test the new type of tanks, the training has a special exercise, its essence is as follows.</p><p>Initially, the column consists of <span class="tex-span"><i>n</i></span> tanks sequentially numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in the order of position in the column from its beginning to its end. During the whole exercise, exactly <span class="tex-span"><i>n</i></span> messages must be transferred from the beginning of the column to its end.</p><p>Transferring one message is as follows. The tank that goes first in the column transmits the message to some tank in the column. The tank which received the message sends it further down the column. The process is continued until the last tank receives the message. It is possible that not all tanks in the column will receive the message — it is important that the last tank in the column should receive the message.</p><p>After the last tank (tank number <span class="tex-span"><i>n</i></span>) receives the message, it moves to the beginning of the column and sends another message to the end of the column in the same manner. When the message reaches the last tank (tank number <span class="tex-span"><i>n</i> - 1</span>), that tank moves to the beginning of the column and sends the next message to the end of the column, and so on. Thus, the exercise is completed when the tanks in the column return to their original order, that is, immediately after tank number <span class="tex-span">1</span> moves to the beginning of the column.</p><p>If the tanks were initially placed in the column in the order <span class="tex-span">1, 2, ..., <i>n</i></span>, then after the first message their order changes to <span class="tex-span"><i>n</i>, 1, ..., <i>n</i> - 1</span>, after the second message it changes to <span class="tex-span"><i>n</i> - 1, <i>n</i>, 1, ..., <i>n</i> - 2</span>, and so on.</p><p>The tanks are constructed in a very peculiar way. The tank with number <span class="tex-span"><i>i</i></span> is characterized by one integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, which is called the <span class="tex-font-style-underline">message receiving radius</span> of this tank.</p><p>Transferring a message between two tanks takes one second, however, not always one tank can transmit a message to another one. Let's consider two tanks in the column such that the first of them is the <span class="tex-span"><i>i</i></span>-th in the column counting from the beginning, and the second one is the <span class="tex-span"><i>j</i></span>-th in the column, and suppose the second tank has number <span class="tex-span"><i>x</i></span>. Then the first tank can transmit a message to the second tank if <span class="tex-span"><i>i</i> &lt; <i>j</i></span> and <span class="tex-span"><i>i</i> ≥ <i>j</i> - <i>a</i><sub class="lower-index"><i>x</i></sub></span>.</p><p>The Ministry of Defense (and soon the Smart Beaver) faced the question of how to organize the training efficiently. The exercise should be finished as quickly as possible. We'll neglect the time that the tanks spend on moving along the column, since improving the tanks' speed is not a priority for this training.</p><p>You are given the number of tanks, as well as the message receiving radii of all tanks. You must help the Smart Beaver and organize the transferring of messages in a way that makes the total transmission time of all messages as small as possible.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> — the number of tanks in the column. Each of the next <span class="tex-span"><i>n</i></span> lines contains one integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 250000</span>, <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) — the message receiving radii of the tanks in the order from tank <span class="tex-span">1</span> to tank <span class="tex-span"><i>n</i></span> (let us remind you that initially the tanks are located in the column in ascending order of their numbers).</p><p>To get the full points for the first group of tests it is sufficient to solve the problem with <span class="tex-span">2 ≤ <i>n</i> ≤ 300</span>.</p><p>To get the full points for the second group of tests it is sufficient to solve the problem with <span class="tex-span">2 ≤ <i>n</i> ≤ 10000</span>.</p><p>To get the full points for the third group of tests it is sufficient to solve the problem with <span class="tex-span">2 ≤ <i>n</i> ≤ 250000</span>.</p></div><div class="output-specification"><p>Print a single integer — the minimum possible total time of transmitting the messages.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> — the number of tanks in the column. Each of the next <span class="tex-span"><i>n</i></span> lines contains one integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 250000</span>, <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) — the message receiving radii of the tanks in the order from tank <span class="tex-span">1</span> to tank <span class="tex-span"><i>n</i></span> (let us remind you that initially the tanks are located in the column in ascending order of their numbers).</p><p>To get the full points for the first group of tests it is sufficient to solve the problem with <span class="tex-span">2 ≤ <i>n</i> ≤ 300</span>.</p><p>To get the full points for the second group of tests it is sufficient to solve the problem with <span class="tex-span">2 ≤ <i>n</i> ≤ 10000</span>.</p><p>To get the full points for the third group of tests it is sufficient to solve the problem with <span class="tex-span">2 ≤ <i>n</i> ≤ 250000</span>.</p>

## Output

<p>Print a single integer — the minimum possible total time of transmitting the messages.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
3
2
1
1

```




```input2
5
2
2
2
2
2

```




```output1
5

```




```output2
10

```



## Note

<p>In the first sample the original order of tanks is <span class="tex-span">1, 2, 3</span>. The first tank sends a message to the second one, then the second tank sends it to the third one — it takes two seconds. The third tank moves to the beginning of the column and the order of tanks now is <span class="tex-span">3, 1, 2</span>. The third tank sends a message to the first one, then the first one sends it to the second one — it takes two more seconds. The second tank moves to the beginning and the order of the tanks is now <span class="tex-span">2, 3, 1</span>. With this arrangement, the second tank can immediately send a message to the first one, since the message receiving radius of the first tank is large enough — it takes one second. Finally, the tanks return to their original order <span class="tex-span">1, 2, 3</span>. In total, the exercise takes <span class="tex-span">5</span> seconds.</p><p>In the second sample, all five tanks are the same and sending a single message takes two seconds, so in total the exercise takes <span class="tex-span">10</span> seconds.</p>
