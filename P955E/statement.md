## Description

<div><p>Andrew's favourite Krakozyabra has recenly fled away and now he's eager to bring it back!</p><p>At the moment the refugee is inside an icy cave with <span class="tex-span"><i>n</i></span> icicles dangling from the ceiling located in integer coordinates numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The distance between floor and the <span class="tex-span"><i>i</i></span>-th icicle is equal to <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Andrew is free to choose an arbitrary integer point <span class="tex-span"><i>T</i></span> in range from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> inclusive and at time instant <span class="tex-span">0</span> launch a sound wave spreading into both sides (left and right) at the speed of one point per second. Any icicle touched by the wave starts falling at the same speed (that means that in a second the distance from floor to icicle decreases by one but cannot become less that zero). While distance from icicle to floor is more than zero, it is considered passable; as soon as it becomes zero, the icicle blocks the path and prohibits passing.</p><p>Krakozyabra is initially (i.e. at time instant <span class="tex-span">0</span>) is located at point <img align="middle" class="tex-formula" src="file://xKJKWpLg.png" style="max-width: 100.0%;max-height: 100.0%;"> and starts running in the right direction at the speed of one point per second. You can assume that events in a single second happen in the following order: first Krakozyabra changes its position, and only then the sound spreads and icicles fall; in particular, that means that if Krakozyabra is currently at point <img align="middle" class="tex-formula" src="file://YdLJiuZX.png" style="max-width: 100.0%;max-height: 100.0%;"> and the falling (i.e. already touched by the sound wave) icicle at point <span class="tex-span"><i>i</i></span> is <span class="tex-span">1</span> point from the floor, then Krakozyabra will pass it and find itself at <img align="middle" class="tex-formula" src="file://UoJcguWr.png" style="max-width: 100.0%;max-height: 100.0%;"> and only after that the icicle will finally fall and block the path.</p><p>Krakozyabra is considered entrapped if there are fallen (i.e. with <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 0</span>) icicles both to the left and to the right of its current position. Help Andrew find the minimum possible time it takes to entrap Krakozyabra by choosing the optimal value of <span class="tex-span"><i>T</i></span> or report that this mission is impossible.</p></div><div class="input-specification"><p>The first line contains the number of icicles <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p><p>The next line contains <span class="tex-span"><i>n</i></span> space-separated numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span>&nbsp;— the distances from floor to icicles.</p></div><div class="output-specification"><p>Print an only integer — the minimum time it takes to entrap Krakozyabra between two fallen icicles. If it is impossible, print <span class="tex-span"> - 1</span>.</p></div>

## Input

<p>The first line contains the number of icicles <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p><p>The next line contains <span class="tex-span"><i>n</i></span> space-separated numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span>&nbsp;— the distances from floor to icicles.</p>

## Output

<p>Print an only integer — the minimum time it takes to entrap Krakozyabra between two fallen icicles. If it is impossible, print <span class="tex-span"> - 1</span>.</p>





```input1
5
1 4 3 5 1

```




```input2
4
1 2 1 1

```




```input3
2
2 1

```




```input4
2
1 2

```




```output1
3

```




```output2
2

```




```output3
3

```




```output4
-1

```



## Note

<p>In sample case one it's optimal to launch the sound wave from point <span class="tex-span">3</span>. Then in two seconds icicles <span class="tex-span">1</span> and <span class="tex-span">5</span> will start falling, and in one more seconds they will block the paths. Krakozyabra will be located at <img align="middle" class="tex-formula" src="file://XEjTnqPI.png" style="max-width: 100.0%;max-height: 100.0%;"> at that time. Note that icicle number <span class="tex-span">3</span> will also be fallen, so there will actually be two icicles blocking the path to the left.</p><p>In sample case two it is optimal to launch the wave from point <span class="tex-span">2</span> and entrap Krakozyabra in <span class="tex-span">2</span> seconds.</p><p>In sample case four the answer is impossible.</p>
