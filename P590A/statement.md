## Description

<div><p>A schoolboy named Vasya loves reading books on programming and mathematics. He has recently read an encyclopedia article that described the method of <span class="tex-font-style-it">median smoothing</span> (or median filter) and its many applications in science and engineering. Vasya liked the idea of the method very much, and he decided to try it in practice.</p><p>Applying the simplest variant of median smoothing to the sequence of numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> will result a new sequence <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> obtained by the following algorithm:</p><ul> <li> <span class="tex-span"><i>b</i><sub class="lower-index">1</sub> = <i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>n</i></sub> = <i>a</i><sub class="lower-index"><i>n</i></sub></span>, that is, the first and the last number of the new sequence match the corresponding numbers of the original sequence. </li><li> For <span class="tex-span"><i>i</i> = 2, ..., <i>n</i> - 1</span> value <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is equal to the <span class="tex-font-style-it">median</span> of three values <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i> - 1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i> + 1</sub></span>. </li></ul><p>The <span class="tex-font-style-it">median</span> of a set of three numbers is the number that goes on the second place, when these three numbers are written in the non-decreasing order. For example, the median of the set 5, 1, 2 is number 2, and the median of set 1, 0, 1 is equal to 1.</p><p>In order to make the task easier, Vasya decided to apply the method to sequences consisting of zeros and ones only.</p><p>Having made the procedure once, Vasya looked at the resulting sequence and thought: what if I apply the algorithm to it once again, and then apply it to the next result, and so on? Vasya tried a couple of examples and found out that after some number of median smoothing algorithm applications the sequence can stop changing. We say that the sequence is <span class="tex-font-style-it">stable</span>, if it does not change when the median smoothing is applied to it.</p><p>Now Vasya wonders, whether the sequence always eventually becomes stable. He asks you to write a program that, given a sequence of zeros and ones, will determine whether it ever becomes stable. Moreover, if it ever becomes stable, then you should determine what will it look like and how many times one needs to apply the median smoothing algorithm to initial sequence in order to obtain a stable one.</p></div><div class="input-specification"><p>The first input line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 500 000</span>)&nbsp;— the length of the initial sequence.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 0</span> or <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 1</span>), giving the initial sequence itself.</p></div><div class="output-specification"><p>If the sequence will never become stable, print a single number <span class="tex-span"> - 1</span>.</p><p>Otherwise, first print a single integer&nbsp;— the minimum number of times one needs to apply the median smoothing algorithm to the initial sequence before it becomes is stable. In the second line print <span class="tex-span"><i>n</i></span> numbers separated by a space &nbsp;— the resulting sequence itself.</p></div>

## Input

<p>The first input line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 500 000</span>)&nbsp;— the length of the initial sequence.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 0</span> or <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 1</span>), giving the initial sequence itself.</p>

## Output

<p>If the sequence will never become stable, print a single number <span class="tex-span"> - 1</span>.</p><p>Otherwise, first print a single integer&nbsp;— the minimum number of times one needs to apply the median smoothing algorithm to the initial sequence before it becomes is stable. In the second line print <span class="tex-span"><i>n</i></span> numbers separated by a space &nbsp;— the resulting sequence itself.</p>





```input1
4
0 0 1 1

```




```input2
5
0 1 0 1 0

```




```output1
0
0 0 1 1

```




```output2
2
0 0 0 0 0

```



## Note

<p>In the second sample the stabilization occurs in two steps: <img align="middle" class="tex-formula" src="file://WX7El5Or.png" style="max-width: 100.0%;max-height: 100.0%;">, and the sequence <span class="tex-span">00000</span> is obviously stable.</p>
