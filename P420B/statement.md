## Description

<div><p>Nearly each project of the F company has a whole team of developers working on it. They often are in different rooms of the office in different cities and even countries. To keep in touch and track the results of the project, the F company conducts shared online meetings in a Spyke chat.</p><p>One day the director of the F company got hold of the records of a part of an online meeting of one successful team. The director watched the record and wanted to talk to the team leader. But how can he tell who the leader is? The director logically supposed that the leader is the person who is present at any conversation during a chat meeting. In other words, if at some moment of time at least one person is present on the meeting, then the leader is present on the meeting.</p><p>You are the assistant director. Given the 'user logged on'/'user logged off' messages of the meeting in the chronological order, help the director determine who can be the leader. Note that the director has the record of only a continuous part of the meeting (probably, it's not the whole meeting).</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of team participants and the number of messages. Each of the next <span class="tex-span"><i>m</i></span> lines contains a message in the format:</p><ul> <li> '<span class="tex-font-style-tt">+ </span><span class="tex-span"><i>id</i></span>': the record means that the person with number <span class="tex-span"><i>id</i></span> <span class="tex-span">(1 ≤ <i>id</i> ≤ <i>n</i>)</span> has logged on to the meeting. </li><li> '<span class="tex-font-style-tt">- </span><span class="tex-span"><i>id</i></span>': the record means that the person with number <span class="tex-span"><i>id</i></span> <span class="tex-span">(1 ≤ <i>id</i> ≤ <i>n</i>)</span> has logged off from the meeting. </li></ul><p>Assume that all the people of the team are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> and the messages are given in the chronological order. It is guaranteed that the given sequence is the correct record of a continuous part of the meeting. It is guaranteed that no two log on/log off events occurred simultaneously.</p></div><div class="output-specification"><p>In the first line print integer <span class="tex-span"><i>k</i></span> <span class="tex-span">(0 ≤ <i>k</i> ≤ <i>n</i>)</span> — how many people can be leaders. In the next line, print <span class="tex-span"><i>k</i></span> integers in the increasing order — the numbers of the people who can be leaders.</p><p>If the data is such that no member of the team can be a leader, print a single number <span class="tex-span">0</span>.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of team participants and the number of messages. Each of the next <span class="tex-span"><i>m</i></span> lines contains a message in the format:</p><ul> <li> '<span class="tex-font-style-tt">+ </span><span class="tex-span"><i>id</i></span>': the record means that the person with number <span class="tex-span"><i>id</i></span> <span class="tex-span">(1 ≤ <i>id</i> ≤ <i>n</i>)</span> has logged on to the meeting. </li><li> '<span class="tex-font-style-tt">- </span><span class="tex-span"><i>id</i></span>': the record means that the person with number <span class="tex-span"><i>id</i></span> <span class="tex-span">(1 ≤ <i>id</i> ≤ <i>n</i>)</span> has logged off from the meeting. </li></ul><p>Assume that all the people of the team are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> and the messages are given in the chronological order. It is guaranteed that the given sequence is the correct record of a continuous part of the meeting. It is guaranteed that no two log on/log off events occurred simultaneously.</p>

## Output

<p>In the first line print integer <span class="tex-span"><i>k</i></span> <span class="tex-span">(0 ≤ <i>k</i> ≤ <i>n</i>)</span> — how many people can be leaders. In the next line, print <span class="tex-span"><i>k</i></span> integers in the increasing order — the numbers of the people who can be leaders.</p><p>If the data is such that no member of the team can be a leader, print a single number <span class="tex-span">0</span>.</p>





```input1
5 4
+ 1
+ 2
- 2
- 1

```




```input2
3 2
+ 1
- 2

```




```input3
2 4
+ 1
- 1
+ 2
- 2

```




```input4
5 6
+ 1
- 1
- 3
+ 3
+ 4
- 4

```




```input5
2 4
+ 1
- 2
+ 2
- 1

```




```output1
4
1 3 4 5
```




```output2
1
3
```




```output3
0

```




```output4
3
2 3 5
```




```output5
0

```


