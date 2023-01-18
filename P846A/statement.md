## Description

<div><p>Hideo Kojima has just quit his job at Konami. Now he is going to find a new place to work. Despite being such a well-known person, he still needs a CV to apply for a job.</p><p>During all his career Hideo has produced <span class="tex-span"><i>n</i></span> games. Some of them were successful, some were not. Hideo wants to remove several of them (possibly zero) from his CV to make a better impression on employers. As a result there should be no unsuccessful game which comes right after successful one in his CV.</p><p>More formally, you are given an array <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i></sub></span> of zeros and ones. Zero corresponds to an unsuccessful game, one — to a successful one. Games are given in order they were produced, and Hideo can't swap these values. He should remove some elements from this array in such a way that no zero comes right after one.</p><p>Besides that, Hideo still wants to mention as much games in his CV as possible. Help this genius of a man determine the maximum number of games he can leave in his CV.</p></div><div class="input-specification"><p>The first line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integer numbers <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>). <span class="tex-span">0</span> corresponds to an unsuccessful game, <span class="tex-span">1</span> — to a successful one.</p></div><div class="output-specification"><p>Print one integer — the maximum number of games Hideo can leave in his CV so that no unsuccessful game comes after a successful one.</p></div>

## Input

<p>The first line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integer numbers <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>). <span class="tex-span">0</span> corresponds to an unsuccessful game, <span class="tex-span">1</span> — to a successful one.</p>

## Output

<p>Print one integer — the maximum number of games Hideo can leave in his CV so that no unsuccessful game comes after a successful one.</p>





```input1
4
1 1 0 1

```




```input2
6
0 1 0 0 1 0

```




```input3
1
0

```




```output1
3

```




```output2
4

```




```output3
1

```


