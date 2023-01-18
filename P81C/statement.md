## Description

<div><p>After the educational reform Polycarp studies only two subjects at school, Safety Studies and PE (Physical Education). During the long months of the fourth term, he received <span class="tex-span"><i>n</i></span> marks in them. When teachers wrote a mark in the journal, they didn't write in what subject the mark was for, they just wrote the mark.</p><p>Now it's time to show the journal to his strict parents. Polycarp knows that recently at the Parent Meeting the parents were told that he received <span class="tex-span"><i>a</i></span> Safety Studies marks and <span class="tex-span"><i>b</i></span> PE marks (<span class="tex-span"><i>a</i> + <i>b</i> = <i>n</i></span>). Now Polycarp wants to write a subject's name in front of each mark so that: </p><ul> <li> there are exactly <span class="tex-span"><i>a</i></span> Safety Studies marks, </li><li> there are exactly <span class="tex-span"><i>b</i></span> PE marks, </li><li> the total average score in both subjects is maximum. </li></ul><p>An average subject grade is the sum of all marks in it, divided by the number of them. Of course, the division is performed in real numbers without rounding up or down. Polycarp aims to maximize the <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> + <i>x</i><sub class="lower-index">2</sub></span>, where <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> is the average score in the first subject (Safety Studies), and <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> is the average score in the second one (Physical Education).</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), <span class="tex-span"><i>n</i></span> is the number of marks in Polycarp's Journal. The second line contains two positive integers <span class="tex-span"><i>a</i>, <i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i> - 1, <i>a</i> + <i>b</i> = <i>n</i></span>). The third line contains a sequence of integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 5</span>), they are Polycarp's marks.</p></div><div class="output-specification"><p>Print the sequence of integers <span class="tex-span"><i>f</i><sub class="lower-index">1</sub>, <i>f</i><sub class="lower-index">2</sub>, ..., <i>f</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>f</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>) is the number of a subject to which the <span class="tex-span"><i>i</i></span>-th mark should be attributed. If there are several possible solutions, then print such that the sequence <span class="tex-span"><i>f</i><sub class="lower-index">1</sub>, <i>f</i><sub class="lower-index">2</sub>, ..., <i>f</i><sub class="lower-index"><i>n</i></sub></span> is the smallest lexicographically.</p><p>The sequence <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> is lexicographically less than <span class="tex-span"><i>q</i><sub class="lower-index">1</sub>, <i>q</i><sub class="lower-index">2</sub>, ..., <i>q</i><sub class="lower-index"><i>n</i></sub></span> if there exists such <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>n</i></span>) that <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> = <i>q</i><sub class="lower-index"><i>i</i></sub></span> for all <span class="tex-span">1 ≤ <i>i</i> &lt; <i>j</i></span>, аnd <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub> &lt; <i>q</i><sub class="lower-index"><i>j</i></sub></span>.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), <span class="tex-span"><i>n</i></span> is the number of marks in Polycarp's Journal. The second line contains two positive integers <span class="tex-span"><i>a</i>, <i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i> - 1, <i>a</i> + <i>b</i> = <i>n</i></span>). The third line contains a sequence of integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 5</span>), they are Polycarp's marks.</p>

## Output

<p>Print the sequence of integers <span class="tex-span"><i>f</i><sub class="lower-index">1</sub>, <i>f</i><sub class="lower-index">2</sub>, ..., <i>f</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>f</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>) is the number of a subject to which the <span class="tex-span"><i>i</i></span>-th mark should be attributed. If there are several possible solutions, then print such that the sequence <span class="tex-span"><i>f</i><sub class="lower-index">1</sub>, <i>f</i><sub class="lower-index">2</sub>, ..., <i>f</i><sub class="lower-index"><i>n</i></sub></span> is the smallest lexicographically.</p><p>The sequence <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> is lexicographically less than <span class="tex-span"><i>q</i><sub class="lower-index">1</sub>, <i>q</i><sub class="lower-index">2</sub>, ..., <i>q</i><sub class="lower-index"><i>n</i></sub></span> if there exists such <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>n</i></span>) that <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> = <i>q</i><sub class="lower-index"><i>i</i></sub></span> for all <span class="tex-span">1 ≤ <i>i</i> &lt; <i>j</i></span>, аnd <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub> &lt; <i>q</i><sub class="lower-index"><i>j</i></sub></span>.</p>





```input1
5
3 2
4 4 5 4 4

```




```input2
4
2 2
3 5 4 5

```




```input3
6
1 5
4 4 4 5 4 4

```




```output1
1 1 2 1 2
```




```output2
1 1 2 2
```




```output3
2 2 2 1 2 2
```



## Note

<p>In the first sample the average score in the first subject is equal to 4, and in the second one — to 4.5. The total average score is 8.5.</p>
