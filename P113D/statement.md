## Description

<div><p>One day as Petya and his friend Vasya were having one of their numerous trips, they decided to visit a museum castle. The museum has a specific shape: it consists of <span class="tex-span"><i>n</i></span> rooms connected with <span class="tex-span"><i>m</i></span> corridors so that one can access any room from any other one.</p><p>After the two friends had a little walk around the museum, they decided to split and watch the pieces of art each of them found interesting. They agreed to meet in one of the rooms at six p.m. However, they forgot one quite essential thing: they didn't specify the place to meet and when the time came, they started to rush about the museum looking for each other (they couldn't call each other as roaming made a call's cost skyrocket).</p><p>Yet, even despite the whole rush, they couldn't get enough of the pieces of art, that's why each of them has the following strategy: each minute he make a decision where to go — with probability <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> he doesn't move to any other place during this minute (i.e. he stays in the room). With probability <span class="tex-span">1 - <i>p</i><sub class="lower-index"><i>i</i></sub></span> he equiprobably choose one of the adjacent rooms and went there along the corridor. Here <span class="tex-span"><i>i</i></span> is the ordinal number of the current room. Building was expensive in ancient times, that's why each corridor connected two different rooms, and any two rooms had no more than one corridor between them. </p><p>The boys act simultaneously. As the corridors are dark, it is impossible to meet there; however, one can walk along the corridors in both directions (besides, the two boys can be going through the same corridor simultaneously without meeting). The boys act like that until they meet each other. More formally, the two friends meet when at some moment of time both of them decided to appear in the same room.</p><p>For each room find the probability that the boys will meet there considering that at 6 p.m. they are positioned in rooms <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> correspondingly.</p></div><div class="input-specification"><p>The first line contains four integers: <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 22)</span>, representing the numbers of rooms; <span class="tex-span"><i>m</i></span> <img align="middle" class="tex-formula" src="file://YqoTEo2d.png" style="max-width: 100.0%;max-height: 100.0%;">, representing the number of corridors; <span class="tex-span"><i>a</i>, <i>b</i></span> <span class="tex-span">(1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i>)</span>, representing the numbers of Petya's and Vasya's starting rooms correspondingly.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain pairs of numbers — the numbers of rooms connected by a corridor. Next <span class="tex-span"><i>n</i></span> lines contain probabilities <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0.01 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 0.99)</span> with the accuracy of up to four digits after the decimal point — the probability to stay in room <span class="tex-span"><i>i</i></span>.</p><p>It is guaranteed that every room can be reached from every other room by corridors.</p></div><div class="output-specification"><p>In the only line print <span class="tex-span"><i>n</i></span> space-separated numbers, the <span class="tex-span"><i>i</i></span>-th number should represent the probability that the friends meet in the <span class="tex-span"><i>i</i></span>-th room with absolute or relative error of no more than <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line contains four integers: <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 22)</span>, representing the numbers of rooms; <span class="tex-span"><i>m</i></span> <img align="middle" class="tex-formula" src="file://YqoTEo2d.png" style="max-width: 100.0%;max-height: 100.0%;">, representing the number of corridors; <span class="tex-span"><i>a</i>, <i>b</i></span> <span class="tex-span">(1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i>)</span>, representing the numbers of Petya's and Vasya's starting rooms correspondingly.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain pairs of numbers — the numbers of rooms connected by a corridor. Next <span class="tex-span"><i>n</i></span> lines contain probabilities <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0.01 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 0.99)</span> with the accuracy of up to four digits after the decimal point — the probability to stay in room <span class="tex-span"><i>i</i></span>.</p><p>It is guaranteed that every room can be reached from every other room by corridors.</p>

## Output

<p>In the only line print <span class="tex-span"><i>n</i></span> space-separated numbers, the <span class="tex-span"><i>i</i></span>-th number should represent the probability that the friends meet in the <span class="tex-span"><i>i</i></span>-th room with absolute or relative error of no more than <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
2 1 1 2
1 2
0.5
0.5

```




```input2
4 4 1 2
1 2
2 3
3 4
4 1
0.5
0.5
0.5
0.5

```




```output1
0.5000000000 0.5000000000
```




```output2
0.3333333333 0.3333333333 0.1666666667 0.1666666667
```



## Note

<p>In the first sample the museum is symmetric. That means the probabilities to meet in rooms 1 and 2 are equal. And their sum equals to one. So, each probability equals <span class="tex-span">0.5</span>.</p>
