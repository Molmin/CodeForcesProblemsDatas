## Description

<div><p>In the Main Berland Bank <span class="tex-span"><i>n</i></span> people stand in a queue at the cashier, everyone knows his/her height <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>, and the heights of the other people in the queue. Each of them keeps in mind number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> — how many people who are taller than him/her and stand in queue in front of him.</p><p>After a while the cashier has a lunch break and the people in the queue seat on the chairs in the waiting room in a random order.</p><p>When the lunch break was over, it turned out that nobody can remember the exact order of the people in the queue, but everyone remembers his number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Your task is to restore the order in which the people stood in the queue if it is possible. There may be several acceptable orders, but you need to find any of them. Also, you need to print a possible set of numbers <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> — the heights of people in the queue, so that the numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> are correct.</p></div><div class="input-specification"><p>The first input line contains integer <span class="tex-span"><i>n</i></span> — the number of people in the queue (<span class="tex-span">1 ≤ <i>n</i> ≤ 3000</span>). Then <span class="tex-span"><i>n</i></span> lines contain descriptions of the people as "<span class="tex-span"><i>name</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>" (one description on one line), where <span class="tex-span"><i>name</i><sub class="lower-index"><i>i</i></sub></span> is a non-empty string consisting of lowercase Latin letters whose length does not exceed <span class="tex-span">10</span> characters (the <span class="tex-span"><i>i</i></span>-th person's name), <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is an integer (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - 1</span>), that represents the number of people who are higher and stand in the queue in front of person <span class="tex-span"><i>i</i></span>. It is guaranteed that all names are different.</p></div><div class="output-specification"><p>If there's no acceptable order of the people in the queue, print the single line containing "<span class="tex-font-style-tt">-1</span>" without the quotes. Otherwise, print in <span class="tex-span"><i>n</i></span> lines the people as "<span class="tex-span"><i>name</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>", where <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> is the integer from <span class="tex-span">1</span> to <span class="tex-span">10<sup class="upper-index">9</sup></span> (inclusive), the possible height of a man whose name is <span class="tex-span"><i>name</i><sub class="lower-index"><i>i</i></sub></span>. Print the people in the order in which they stand in the queue, starting from the head of the queue and moving to its tail. Numbers <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> are not necessarily unique.</p></div>

## Input

<p>The first input line contains integer <span class="tex-span"><i>n</i></span> — the number of people in the queue (<span class="tex-span">1 ≤ <i>n</i> ≤ 3000</span>). Then <span class="tex-span"><i>n</i></span> lines contain descriptions of the people as "<span class="tex-span"><i>name</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>" (one description on one line), where <span class="tex-span"><i>name</i><sub class="lower-index"><i>i</i></sub></span> is a non-empty string consisting of lowercase Latin letters whose length does not exceed <span class="tex-span">10</span> characters (the <span class="tex-span"><i>i</i></span>-th person's name), <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is an integer (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - 1</span>), that represents the number of people who are higher and stand in the queue in front of person <span class="tex-span"><i>i</i></span>. It is guaranteed that all names are different.</p>

## Output

<p>If there's no acceptable order of the people in the queue, print the single line containing "<span class="tex-font-style-tt">-1</span>" without the quotes. Otherwise, print in <span class="tex-span"><i>n</i></span> lines the people as "<span class="tex-span"><i>name</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>", where <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> is the integer from <span class="tex-span">1</span> to <span class="tex-span">10<sup class="upper-index">9</sup></span> (inclusive), the possible height of a man whose name is <span class="tex-span"><i>name</i><sub class="lower-index"><i>i</i></sub></span>. Print the people in the order in which they stand in the queue, starting from the head of the queue and moving to its tail. Numbers <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> are not necessarily unique.</p>





```input1
4
a 0
b 2
c 0
d 0

```




```input2
4
vasya 0
petya 1
manya 3
dunay 3

```




```output1
a 150
c 170
d 180
b 160

```




```output2
-1

```


