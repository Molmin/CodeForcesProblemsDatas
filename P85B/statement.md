## Description

<div><p>In an embassy of a well-known kingdom an electronic queue is organised. Every person who comes to the embassy, needs to make the following three actions: show the ID, pay money to the cashier and be fingerprinted. <span class="tex-font-style-bf">Besides, the actions should be performed in the given order.</span></p><p>For each action several separate windows are singled out: <span class="tex-span"><i>k</i><sub class="lower-index">1</sub></span> separate windows for the first action (the first type windows), <span class="tex-span"><i>k</i><sub class="lower-index">2</sub></span> windows for the second one (the second type windows), and <span class="tex-span"><i>k</i><sub class="lower-index">3</sub></span> for the third one (the third type windows). The service time for one person in any of the first type window equals to <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span>. Similarly, it takes <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span> time to serve a person in any of the second type windows. And it takes <span class="tex-span"><i>t</i><sub class="lower-index">3</sub></span> to serve one person in any of the third type windows. Thus, the service time depends only on the window type and is independent from the person who is applying for visa.</p><p>At some moment <span class="tex-span"><i>n</i></span> people come to the embassy, the <span class="tex-span"><i>i</i></span>-th person comes at the moment of time <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>. The person is registered under some number. After that he sits in the hall and waits for his number to be shown on a special board. Besides the person's number the board shows the number of the window where one should go and the person goes there immediately. Let's consider that the time needed to approach the window is negligible. The table can show information for no more than one person at a time. The electronic queue works so as to immediately start working with the person who has approached the window, as there are no other people in front of the window.</p><p>The Client Service Quality inspectors noticed that several people spend too much time in the embassy (this is particularly tiresome as the embassy has no mobile phone reception and 3G). It was decided to organise the system so that the largest time a person spends in the embassy were minimum. Help the inspectors organise the queue. Consider that all actions except for being served in at the window, happen instantly.</p></div><div class="input-specification"><p>The first line contains three space-separated integers <span class="tex-span"><i>k</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>k</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>k</i><sub class="lower-index">3</sub></span> (<span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), they are the number of windows of the first, second and third type correspondingly.</p><p>The second line contains three space-separated integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index">3</sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>), they are the periods of time needed to serve one person in the window of the first, second and third type correspondingly. </p><p>The third line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), it is the number of people.</p><p>The fourth line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) in the non-decreasing order; <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is the time when the person number <span class="tex-span"><i>i</i></span> comes to the embassy.</p></div><div class="output-specification"><p>Print the single number, the maximum time a person will spend in the embassy if the queue is organized optimally.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams (also you may use the <span class="tex-font-style-tt">%I64d</span> specificator).</p></div>

## Input

<p>The first line contains three space-separated integers <span class="tex-span"><i>k</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>k</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>k</i><sub class="lower-index">3</sub></span> (<span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), they are the number of windows of the first, second and third type correspondingly.</p><p>The second line contains three space-separated integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index">3</sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>), they are the periods of time needed to serve one person in the window of the first, second and third type correspondingly. </p><p>The third line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), it is the number of people.</p><p>The fourth line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) in the non-decreasing order; <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is the time when the person number <span class="tex-span"><i>i</i></span> comes to the embassy.</p>

## Output

<p>Print the single number, the maximum time a person will spend in the embassy if the queue is organized optimally.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams (also you may use the <span class="tex-font-style-tt">%I64d</span> specificator).</p>





```input1
1 1 1
1 1 1
5
1 1 1 1 1

```




```input2
2 1 1
5 1 1
5
1 2 3 3 5

```




```output1
7

```




```output2
13

```



## Note

<p>In the first test 5 people come simultaneously at the moment of time equal to 1. There is one window of every type, it takes 1 unit of time to be served at each window. That's why the maximal time a person spends in the embassy is the time needed to be served at the windows (3 units of time) plus the time the last person who comes to the first window waits (4 units of time).</p><p> Windows in the second test work like this:</p><p>The first window of the first type: <span class="tex-span">[1, 6)</span> — the first person, <span class="tex-span">[6, 11)</span> — third person, <span class="tex-span">[11, 16)</span> — fifth person</p><p>The second window of the first type: <span class="tex-span">[2, 7)</span> — the second person, <span class="tex-font-style-bf"><span class="tex-span">[7, 12)</span></span> — the fourth person</p><p>The only second type window: <span class="tex-span">[6, 7)</span> — first, <span class="tex-span">[7, 8)</span> — second, <span class="tex-span">[11, 12)</span> — third, <span class="tex-span">[12, 13)</span> — fourth, <span class="tex-span">[16, 17)</span> — fifth</p><p>The only third type window: <span class="tex-span">[7, 8)</span> — first, <span class="tex-span">[8, 9)</span> — second, <span class="tex-span">[12, 13)</span> — third, <span class="tex-span">[13, 14)</span> — fourth, <span class="tex-span">[17, 18)</span> — fifth</p><p>We can see that it takes most time to serve the fifth person.</p>
