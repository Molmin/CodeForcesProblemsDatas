## Description

<div><p>Polycarpus likes studying at school a lot and he is always diligent about his homework. Polycarpus has never had any problems with natural sciences as his great-great-grandfather was the great physicist Seinstein. On the other hand though, Polycarpus has never had an easy time with history.</p><p>Everybody knows that the World history encompasses exactly <span class="tex-span"><i>n</i></span> events: the <span class="tex-span"><i>i</i></span>-th event had continued from the year <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to the year <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> inclusive (<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub></span>). Polycarpus easily learned the dates when each of <span class="tex-span"><i>n</i></span> events started and ended (Polycarpus inherited excellent memory from his great-great-granddad). But the teacher gave him a more complicated task: Polycaprus should know when all events began and ended and he should also find out for each event whether it includes another event. Polycarpus' teacher thinks that an event <span class="tex-span"><i>j</i></span> includes an event <span class="tex-span"><i>i</i></span> if <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub> &lt; <i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>j</i></sub></span>. Your task is simpler: find the number of events that are included in some other event.</p></div><div class="input-specification"><p>The first input line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) which represents the number of events. Next <span class="tex-span"><i>n</i></span> lines contain descriptions of the historical events, one event per line. The <span class="tex-span"><i>i</i> + 1</span> line contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the beginning and the end of the <span class="tex-span"><i>i</i></span>-th event. No two events start or finish in the same year, that is, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>a</i><sub class="lower-index"><i>j</i></sub>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>j</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≠ <i>a</i><sub class="lower-index"><i>j</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>j</i></sub></span> for all <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>j</i></span> (where <span class="tex-span"><i>i</i> ≠ <i>j</i></span>). Events are given in arbitrary order.</p></div><div class="output-specification"><p>Print the only integer — the answer to the problem.</p></div>

## Input

<p>The first input line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) which represents the number of events. Next <span class="tex-span"><i>n</i></span> lines contain descriptions of the historical events, one event per line. The <span class="tex-span"><i>i</i> + 1</span> line contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the beginning and the end of the <span class="tex-span"><i>i</i></span>-th event. No two events start or finish in the same year, that is, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>a</i><sub class="lower-index"><i>j</i></sub>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>j</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≠ <i>a</i><sub class="lower-index"><i>j</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>j</i></sub></span> for all <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>j</i></span> (where <span class="tex-span"><i>i</i> ≠ <i>j</i></span>). Events are given in arbitrary order.</p>

## Output

<p>Print the only integer — the answer to the problem.</p>





```input1
5
1 10
2 9
3 8
4 7
5 6

```




```input2
5
1 100
2 50
51 99
52 98
10 60

```




```input3
1
1 1000000000

```




```output1
4

```




```output2
4

```




```output3
0

```



## Note

<p>In the first example the fifth event is contained in the fourth. Similarly, the fourth event is contained in the third, the third — in the second and the second — in the first.</p><p>In the second example all events except the first one are contained in the first.</p><p>In the third example only one event, so the answer is 0.</p>
