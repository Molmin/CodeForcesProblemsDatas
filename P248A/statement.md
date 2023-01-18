## Description

<div><p>One foggy Stockholm morning, Karlsson decided to snack on some jam in his friend Lillebror Svantenson's house. Fortunately for Karlsson, there wasn't anybody in his friend's house. Karlsson was not going to be hungry any longer, so he decided to get some food in the house.</p><p>Karlsson's gaze immediately fell on <span class="tex-span"><i>n</i></span> wooden cupboards, standing in the kitchen. He immediately realized that these cupboards have hidden jam stocks. Karlsson began to fly greedily around the kitchen, opening and closing the cupboards' doors, grab and empty all the jars of jam that he could find.</p><p>And now all jars of jam are empty, Karlsson has had enough and does not want to leave traces of his stay, so as not to let down his friend. Each of the cupboards has two doors: the left one and the right one. Karlsson remembers that when he rushed to the kitchen, all the cupboards' left doors were in the same position (open or closed), similarly, all the cupboards' right doors were in the same position (open or closed). Karlsson wants the doors to meet this condition as well by the time the family returns. Karlsson does not remember the position of all the left doors, also, he cannot remember the position of all the right doors. Therefore, it does not matter to him in what position will be all left or right doors. It is important to leave all the left doors in the same position, and all the right doors in the same position. For example, all the left doors may be closed, and all the right ones may be open.</p><p>Karlsson needs one second to open or close a door of a cupboard. He understands that he has very little time before the family returns, so he wants to know the minimum number of seconds <span class="tex-span"><i>t</i></span>, in which he is able to bring all the cupboard doors in the required position.</p><p>Your task is to write a program that will determine the required number of seconds <span class="tex-span"><i>t</i></span>.</p></div><div class="input-specification"><p>The first input line contains a single integer <span class="tex-span"><i>n</i></span> — the number of cupboards in the kitchen (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup></span>). Then follow <span class="tex-span"><i>n</i></span> lines, each containing two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 1)</span>. Number <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> equals one, if the left door of the <span class="tex-span"><i>i</i></span>-th cupboard is opened, otherwise number <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> equals zero. Similarly, number <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> equals one, if the right door of the <span class="tex-span"><i>i</i></span>-th cupboard is opened, otherwise number <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> equals zero.</p><p>The numbers in the lines are separated by single spaces.</p></div><div class="output-specification"><p>In the only output line print a single integer <span class="tex-span"><i>t</i></span> — the minimum number of seconds Karlsson needs to change the doors of all cupboards to the position he needs.</p></div>

## Input

<p>The first input line contains a single integer <span class="tex-span"><i>n</i></span> — the number of cupboards in the kitchen (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup></span>). Then follow <span class="tex-span"><i>n</i></span> lines, each containing two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 1)</span>. Number <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> equals one, if the left door of the <span class="tex-span"><i>i</i></span>-th cupboard is opened, otherwise number <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> equals zero. Similarly, number <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> equals one, if the right door of the <span class="tex-span"><i>i</i></span>-th cupboard is opened, otherwise number <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> equals zero.</p><p>The numbers in the lines are separated by single spaces.</p>

## Output

<p>In the only output line print a single integer <span class="tex-span"><i>t</i></span> — the minimum number of seconds Karlsson needs to change the doors of all cupboards to the position he needs.</p>





```input1
5
0 1
1 0
0 1
1 1
0 1

```




```output1
3

```


