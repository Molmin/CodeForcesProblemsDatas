## Description

<div><p>There are <span class="tex-span"><i>n</i></span> incoming messages for Vasya. The <span class="tex-span"><i>i</i></span>-th message is going to be received after <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> minutes. Each message has a cost, which equals to <span class="tex-span"><i>A</i></span> initially. After being received, the cost of a message decreases by <span class="tex-span"><i>B</i></span> each minute (it can become negative). Vasya can read any message after receiving it at any moment of time. After reading the message, Vasya's bank account receives the current cost of this message. Initially, Vasya's bank account is at <span class="tex-span">0</span>.</p><p>Also, each minute Vasya's bank account receives <span class="tex-span"><i>C</i>·<i>k</i></span>, where <span class="tex-span"><i>k</i></span> is the amount of received but unread messages.</p><p>Vasya's messages are very important to him, and because of that he wants to have all messages read after <span class="tex-span"><i>T</i></span> minutes.</p><p>Determine the maximum amount of money Vasya's bank account can hold after <span class="tex-span"><i>T</i></span> minutes.</p></div><div class="input-specification"><p>The first line contains five integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>A</i></span>, <span class="tex-span"><i>B</i></span>, <span class="tex-span"><i>C</i></span> and <span class="tex-span"><i>T</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>A</i>, <i>B</i>, <i>C</i>, <i>T</i> ≤ 1000</span>).</p><p>The second string contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ <i>T</i></span>).</p></div><div class="output-specification"><p>Output one integer &nbsp;— the answer to the problem.</p></div>

## Input

<p>The first line contains five integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>A</i></span>, <span class="tex-span"><i>B</i></span>, <span class="tex-span"><i>C</i></span> and <span class="tex-span"><i>T</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>A</i>, <i>B</i>, <i>C</i>, <i>T</i> ≤ 1000</span>).</p><p>The second string contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ <i>T</i></span>).</p>

## Output

<p>Output one integer &nbsp;— the answer to the problem.</p>





```input1
4 5 5 3 5
1 5 5 4

```




```input2
5 3 1 1 3
2 2 2 1 1

```




```input3
5 5 3 4 5
1 2 3 4 5

```




```output1
20

```




```output2
15

```




```output3
35

```



## Note

<p>In the first sample the messages must be read immediately after receiving, Vasya receives <span class="tex-span"><i>A</i></span> points for each message, <span class="tex-span"><i>n</i>·<i>A</i> = 20</span> in total.</p><p>In the second sample the messages can be read at any integer moment.</p><p>In the third sample messages must be read at the moment T. This way Vasya has <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">3</span>, <span class="tex-span">4</span> and <span class="tex-span">0</span> unread messages at the corresponding minutes, he gets <span class="tex-span">40</span> points for them. When reading messages, he receives <span class="tex-span">(5 - 4·3) + (5 - 3·3) + (5 - 2·3) + (5 - 1·3) + 5 =  - 5</span> points. This is <span class="tex-span">35</span> in total.</p>
