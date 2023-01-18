## Description

<div><p>It seems that Borya is seriously sick. He is going visit <span class="tex-span"><i>n</i></span> doctors to find out the exact diagnosis. Each of the doctors needs the information about all previous visits, so Borya has to visit them in the prescribed order (i.e. Borya should first visit doctor <span class="tex-span">1</span>, then doctor <span class="tex-span">2</span>, then doctor <span class="tex-span">3</span> and so on). Borya will get the information about his health from the last doctor.</p><p>Doctors have a strange working schedule. The doctor <span class="tex-span"><i>i</i></span> goes to work on the <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>-th day and works every <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> day. So, he works on days <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub>, <i>s</i><sub class="lower-index"><i>i</i></sub> + <i>d</i><sub class="lower-index"><i>i</i></sub>, <i>s</i><sub class="lower-index"><i>i</i></sub> + 2<i>d</i><sub class="lower-index"><i>i</i></sub>, ...</span>.</p><p>The doctor's appointment takes quite a long time, so Borya can not see more than one doctor per day. What is the minimum time he needs to visit all doctors?</p></div><div class="input-specification"><p>First line contains an integer <span class="tex-span"><i>n</i></span> — number of doctors (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>). </p><p>Next <span class="tex-span"><i>n</i></span> lines contain two numbers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>).</p></div><div class="output-specification"><p>Output a single integer — the minimum day at which Borya can visit the last doctor.</p></div>

## Input

<p>First line contains an integer <span class="tex-span"><i>n</i></span> — number of doctors (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>). </p><p>Next <span class="tex-span"><i>n</i></span> lines contain two numbers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>).</p>

## Output

<p>Output a single integer — the minimum day at which Borya can visit the last doctor.</p>





```input1
3
2 2
1 2
2 2

```




```input2
2
10 1
6 5

```




```output1
4

```




```output2
11

```



## Note

<p>In the first sample case, Borya can visit all doctors on days <span class="tex-span">2</span>, <span class="tex-span">3</span> and <span class="tex-span">4</span>.</p><p>In the second sample case, Borya can visit all doctors on days <span class="tex-span">10</span> and <span class="tex-span">11</span>.</p>
