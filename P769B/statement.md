## Description

<div><p>Polycarp studies at the university in the group which consists of <span class="tex-span"><i>n</i></span> students (including himself). All they are registrated in the social net "TheContacnt!".</p><p>Not all students are equally sociable. About each student you know the value <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> — the maximum number of messages which the <span class="tex-span"><i>i</i></span>-th student is agree to send per day. The student can't send messages to himself. </p><p>In early morning Polycarp knew important news that the programming credit will be tomorrow. For this reason it is necessary to urgently inform all groupmates about this news using private messages. </p><p>Your task is to make a plan of using private messages, so that:</p><ul> <li> the student <span class="tex-span"><i>i</i></span> sends no more than <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> messages (for all <span class="tex-span"><i>i</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>); </li><li> all students knew the news about the credit (initially only Polycarp knew it); </li><li> the student can inform the other student only if he knows it himself. </li></ul><p>Let's consider that all students are numerated by distinct numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, and Polycarp <span class="tex-font-style-bf">always</span> has the number <span class="tex-span">1</span>.</p><p>In that task you shouldn't minimize the number of messages, the moment of time, when all knew about credit or some other parameters. Find any way how to use private messages which satisfies requirements above. </p></div><div class="input-specification"><p>The first line contains the positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>) — the number of students. </p><p>The second line contains the sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equals to the maximum number of messages which can the <span class="tex-span"><i>i</i></span>-th student agree to send. Consider that Polycarp <span class="tex-font-style-bf">always</span> has the number <span class="tex-span">1</span>.</p></div><div class="output-specification"><p>Print <span class="tex-font-style-tt">-1</span> to the first line if it is impossible to inform all students about credit. </p><p>Otherwise, in the first line print the integer <span class="tex-span"><i>k</i></span> — the number of messages which will be sent. In each of the next <span class="tex-span"><i>k</i></span> lines print two <span class="tex-font-style-bf">distinct</span> integers <span class="tex-span"><i>f</i></span> and <span class="tex-span"><i>t</i></span>, meaning that the student number <span class="tex-span"><i>f</i></span> sent the message with news to the student number <span class="tex-span"><i>t</i></span>. All messages should be printed in chronological order. It means that the student, who is sending the message, must already know this news. It is assumed that students can receive repeated messages with news of the credit. </p><p>If there are several answers, it is acceptable to print any of them. </p></div>

## Input

<p>The first line contains the positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>) — the number of students. </p><p>The second line contains the sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equals to the maximum number of messages which can the <span class="tex-span"><i>i</i></span>-th student agree to send. Consider that Polycarp <span class="tex-font-style-bf">always</span> has the number <span class="tex-span">1</span>.</p>

## Output

<p>Print <span class="tex-font-style-tt">-1</span> to the first line if it is impossible to inform all students about credit. </p><p>Otherwise, in the first line print the integer <span class="tex-span"><i>k</i></span> — the number of messages which will be sent. In each of the next <span class="tex-span"><i>k</i></span> lines print two <span class="tex-font-style-bf">distinct</span> integers <span class="tex-span"><i>f</i></span> and <span class="tex-span"><i>t</i></span>, meaning that the student number <span class="tex-span"><i>f</i></span> sent the message with news to the student number <span class="tex-span"><i>t</i></span>. All messages should be printed in chronological order. It means that the student, who is sending the message, must already know this news. It is assumed that students can receive repeated messages with news of the credit. </p><p>If there are several answers, it is acceptable to print any of them. </p>





```input1
4
1 2 1 0

```




```input2
6
2 0 1 3 2 0

```




```input3
3
0 2 2

```




```output1
3
1 2
2 4
2 3

```




```output2
6
1 3
3 4
1 2
4 5
5 6
4 6

```




```output3
-1

```



## Note

<p>In the first test Polycarp (the student number <span class="tex-span">1</span>) can send the message to the student number <span class="tex-span">2</span>, who after that can send the message to students number <span class="tex-span">3</span> and <span class="tex-span">4</span>. Thus, all students knew about the credit. </p>
