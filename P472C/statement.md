## Description

<div><p>A way to make a new task is to make it nondeterministic or probabilistic. For example, the hard task of Topcoder SRM 595, Constellation, is the probabilistic version of a convex hull.</p><p>Let's try to make a new task. Firstly we will use the following task. There are <span class="tex-span"><i>n</i></span> people, sort them by their name. It is just an ordinary sorting problem, but we can make it more interesting by adding nondeterministic element. There are <span class="tex-span"><i>n</i></span> people, each person will use either his/her first name or last name as a handle. Can the lexicographical order of the handles be exactly equal to the given permutation <span class="tex-span"><i>p</i></span>?</p><p>More formally, if we denote the handle of the <span class="tex-span"><i>i</i></span>-th person as <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>, then the following condition must hold: <img align="middle" class="tex-formula" src="file://tA7S2IoB.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of people.</p><p>The next <span class="tex-span"><i>n</i></span> lines each contains two strings. The <span class="tex-span"><i>i</i></span>-th line contains strings <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ |<i>f</i><sub class="lower-index"><i>i</i></sub>|, |<i>s</i><sub class="lower-index"><i>i</i></sub>| ≤ 50)</span> — the first name and last name of the <span class="tex-span"><i>i</i></span>-th person. Each string consists only of lowercase English letters. All of the given <span class="tex-span">2<i>n</i></span> strings will be distinct.</p><p>The next line contains <span class="tex-span"><i>n</i></span> distinct integers: <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>.</p></div><div class="output-specification"><p>If it is possible, output "<span class="tex-font-style-tt">YES</span>", otherwise output "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of people.</p><p>The next <span class="tex-span"><i>n</i></span> lines each contains two strings. The <span class="tex-span"><i>i</i></span>-th line contains strings <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ |<i>f</i><sub class="lower-index"><i>i</i></sub>|, |<i>s</i><sub class="lower-index"><i>i</i></sub>| ≤ 50)</span> — the first name and last name of the <span class="tex-span"><i>i</i></span>-th person. Each string consists only of lowercase English letters. All of the given <span class="tex-span">2<i>n</i></span> strings will be distinct.</p><p>The next line contains <span class="tex-span"><i>n</i></span> distinct integers: <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>.</p>

## Output

<p>If it is possible, output "<span class="tex-font-style-tt">YES</span>", otherwise output "<span class="tex-font-style-tt">NO</span>".</p>





```input1
3
gennady korotkevich
petr mitrichev
gaoyuan chen
1 2 3

```




```input2
3
gennady korotkevich
petr mitrichev
gaoyuan chen
3 1 2

```




```input3
2
galileo galilei
nicolaus copernicus
2 1

```




```input4
10
rean schwarzer
fei claussell
alisa reinford
eliot craig
laura arseid
jusis albarea
machias regnitz
sara valestin
emma millstein
gaius worzel
1 2 3 4 5 6 7 8 9 10

```




```input5
10
rean schwarzer
fei claussell
alisa reinford
eliot craig
laura arseid
jusis albarea
machias regnitz
sara valestin
emma millstein
gaius worzel
2 4 9 6 5 7 1 3 8 10

```




```output1
NO

```




```output2
YES

```




```output3
YES

```




```output4
NO

```




```output5
YES

```



## Note

<p>In example 1 and 2, we have 3 people: tourist, Petr and me (cgy4ever). You can see that whatever handle is chosen, I must be the first, then tourist and Petr must be the last.</p><p>In example 3, if Copernicus uses "copernicus" as his handle, everything will be alright.</p>
