## Description

<div><p>Gerald is positioned in an old castle which consists of <span class="tex-span"><i>n</i></span> halls connected with <span class="tex-span"><i>n</i> - 1</span> corridors. It is exactly one way to go from any hall to any other one. Thus, the graph is a tree. Initially, at the moment of time <span class="tex-span">0</span>, Gerald is positioned in hall <span class="tex-span">1</span>. Besides, some other hall of the castle contains the treasure Gerald is looking for. The treasure's position is not known; it can equiprobably be in any of other <span class="tex-span"><i>n</i> - 1</span> halls. Gerald can only find out where the treasure is when he enters the hall with the treasure. That very moment Gerald sees the treasure and the moment is regarded is the moment of achieving his goal. </p><p>The corridors have different lengths. At that, the corridors are considered long and the halls are considered small and well lit. Thus, it is possible not to take the time Gerald spends in the halls into consideration. <span class="tex-font-style-bf">The castle is very old, that's why a corridor collapses at the moment when somebody visits it two times, no matter in which direction.</span> </p><p>Gerald can move around the castle using the corridors; he will go until he finds the treasure. Naturally, Gerald wants to find it as quickly as possible. In other words, he wants to act in a manner that would make the average time of finding the treasure as small as possible. <span class="tex-font-style-bf">Each corridor can be used no more than two times. That's why Gerald chooses the strategy in such a way, so he can visit every hall for sure.</span></p><p>More formally, if the treasure is located in the second hall, then Gerald will find it the moment he enters the second hall for the first time — let it be moment <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span>. If the treasure is in the third hall, then Gerald will find it the moment he enters the third hall for the first time. Let it be the moment of time <span class="tex-span"><i>t</i><sub class="lower-index">3</sub></span>. And so on. Thus, the average time of finding the treasure will be equal to <img align="middle" class="tex-formula" src="file://DOT5JS15.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div><div class="input-specification"><p>The first line contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of halls in the castle. Next <span class="tex-span"><i>n</i> - 1</span> lines each contain three integers. The <span class="tex-span"><i>i</i></span>-th line contains numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — the numbers of halls connected with the <span class="tex-span"><i>i</i></span>-th corridor and the time needed to go along the corridor. Initially Gerald is in the hall number <span class="tex-span">1</span>. It is guaranteed that one can get from any hall to any other one using corridors.</p></div><div class="output-specification"><p>Print the only real number: the sought expectation of time needed to find the treasure. The answer should differ from the right one in no less than <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of halls in the castle. Next <span class="tex-span"><i>n</i> - 1</span> lines each contain three integers. The <span class="tex-span"><i>i</i></span>-th line contains numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — the numbers of halls connected with the <span class="tex-span"><i>i</i></span>-th corridor and the time needed to go along the corridor. Initially Gerald is in the hall number <span class="tex-span">1</span>. It is guaranteed that one can get from any hall to any other one using corridors.</p>

## Output

<p>Print the only real number: the sought expectation of time needed to find the treasure. The answer should differ from the right one in no less than <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
2
1 2 1

```




```input2
4
1 3 2
4 2 1
3 2 3

```




```input3
5
1 2 1
1 3 1
1 4 1
1 5 1

```




```output1
1.0

```




```output2
4.333333333333334

```




```output3
4.0

```



## Note

<p>In the first test the castle only has two halls which means that the treasure is located in the second hall. Gerald will only need one minute to go to the second hall from the first one.</p><p>In the second test Gerald can only go from the first hall to the third one. He can get from the third room to the first one or to the second one, but he has already visited the first hall and can get nowhere from there. Thus, he needs to go to the second hall. He should go to hall 4 from there, because all other halls have already been visited. If the treasure is located in the third hall, Gerald will find it in a minute, if the treasure is located in the second hall, Gerald finds it in two minutes, if the treasure is in the fourth hall, Gerald will find it in three minutes. The average time makes <span class="tex-span">2</span> minutes.</p><p>In the third test Gerald needs to visit <span class="tex-span">4</span> halls: the second, third, fourth and fifth ones. All of them are only reachable from the first hall. Thus, he needs to go to those <span class="tex-span">4</span> halls one by one and return. Gerald will enter the first of those halls in a minute, in the second one — in three minutes, in the third one - in <span class="tex-span">5</span> minutes, in the fourth one - in <span class="tex-span">7</span> minutes. The average time is <span class="tex-span">4</span> minutes. </p>
