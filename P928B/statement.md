## Description

<div><p>There are times you recall a good old friend and everything you've come through together. Luckily there are social networks&nbsp;— they store all your message history making it easy to know what you argued over 10 years ago.</p><p>More formal, your message history is a sequence of messages ordered by time sent numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> where <span class="tex-span"><i>n</i></span> is the total number of messages in the chat.</p><p>Each message might contain a link to an earlier message which it is a reply to. When opening a message <span class="tex-span"><i>x</i></span> or getting a link to it, the dialogue is shown in such a way that <span class="tex-span"><i>k</i></span> previous messages, message <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>k</i></span> next messages are visible (with respect to message <span class="tex-span"><i>x</i></span>). In case there are less than <span class="tex-span"><i>k</i></span> messages somewhere, they are yet all shown.</p><p>Digging deep into your message history, you always read all visible messages and then go by the link in the current message <span class="tex-span"><i>x</i></span> (if there is one) and continue reading in the same manner.</p><p>Determine the number of messages you'll read if your start from message number <span class="tex-span"><i>t</i></span> for all <span class="tex-span"><i>t</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Calculate these numbers independently. If you start with message <span class="tex-span"><i>x</i></span>, the initial configuration is <span class="tex-span"><i>x</i></span> itself, <span class="tex-span"><i>k</i></span> previous and <span class="tex-span"><i>k</i></span> next messages. Messages read multiple times are considered as one.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ <i>n</i></span>) — the total amount of messages and the number of previous and next messages visible.</p><p>The second line features a sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>i</i></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> denotes the <span class="tex-span"><i>i</i></span>-th message link destination or zero, if there's no link from <span class="tex-span"><i>i</i></span>. All messages are listed in chronological order. It's guaranteed that the link from message <span class="tex-span"><i>x</i></span> goes to message with number strictly less than <span class="tex-span"><i>x</i></span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> integers with <span class="tex-span"><i>i</i></span>-th denoting the number of distinct messages you can read starting from message <span class="tex-span"><i>i</i></span> and traversing the links while possible.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ <i>n</i></span>) — the total amount of messages and the number of previous and next messages visible.</p><p>The second line features a sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>i</i></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> denotes the <span class="tex-span"><i>i</i></span>-th message link destination or zero, if there's no link from <span class="tex-span"><i>i</i></span>. All messages are listed in chronological order. It's guaranteed that the link from message <span class="tex-span"><i>x</i></span> goes to message with number strictly less than <span class="tex-span"><i>x</i></span>.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> integers with <span class="tex-span"><i>i</i></span>-th denoting the number of distinct messages you can read starting from message <span class="tex-span"><i>i</i></span> and traversing the links while possible.</p>





```input1
6 0
0 1 1 2 3 2

```




```input2
10 1
0 1 0 3 4 5 2 3 7 0

```




```input3
2 2
0 1

```




```output1
1 2 2 3 3 3 

```




```output2
2 3 3 4 5 6 6 6 8 2 

```




```output3
2 2 

```



## Note

<p>Consider <span class="tex-span"><i>i</i> = 6</span> in sample case one. You will read message <span class="tex-span">6</span>, then <span class="tex-span">2</span>, then <span class="tex-span">1</span> and then there will be no link to go.</p><p>In the second sample case <span class="tex-span"><i>i</i> = 6</span> gives you messages <span class="tex-span">5, 6, 7</span> since <span class="tex-span"><i>k</i> = 1</span>, then <span class="tex-span">4, 5, 6</span>, then <span class="tex-span">2, 3, 4</span> and then the link sequence breaks. The number of distinct messages here is equal to <span class="tex-span">6</span>.</p>
