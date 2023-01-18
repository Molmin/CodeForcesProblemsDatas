## Description

<div><p>The biggest gold mine in Berland consists of <span class="tex-span"><i>n</i></span> caves, connected by <span class="tex-span"><i>n</i> - 1</span> transitions. The entrance to the mine leads to the cave number <span class="tex-span">1</span>, it is possible to go from it to any remaining cave of the mine by moving along the transitions. </p><p>The mine is being developed by the InMine Inc., <span class="tex-span"><i>k</i></span> miners work for it. Each day the corporation sorts miners into caves so that each cave has at most one miner working there. </p><p>For each cave we know the height of its ceiling <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> in meters, and for each miner we know his height <span class="tex-span"><i>s</i><sub class="lower-index"><i>j</i></sub></span>, also in meters. If a miner's height doesn't exceed the height of the cave ceiling where he is, then he can stand there comfortably, otherwise, he has to stoop and that makes him unhappy.</p><p>Unfortunately, miners typically go on strike in Berland, so InMine makes all the possible effort to make miners happy about their work conditions. To ensure that no miner goes on strike, you need make sure that no miner has to stoop at any moment on his way from the entrance to the mine to his cave (in particular, he must be able to stand comfortably in the cave where he works). </p><p>To reach this goal, you can choose exactly one cave and increase the height of its ceiling by several meters. However enlarging a cave is an expensive and complex procedure. That's why InMine Inc. asks you either to determine the minimum number of meters you should raise the ceiling of some cave so that it is be possible to sort the miners into the caves and keep all miners happy with their working conditions or to determine that it is impossible to achieve by raising ceiling in exactly one cave.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>) — the number of caves in the mine.</p><p>Then follows a line consisting of <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>h</i><sub class="lower-index">1</sub>, <i>h</i><sub class="lower-index">2</sub>, ..., <i>h</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> is the height of the ceiling in the <span class="tex-span"><i>i</i></span>-th cave.</p><p>Next <span class="tex-span"><i>n</i> - 1</span> lines contain the descriptions of transitions between the caves. Each line has the form <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are the numbers of the caves connected by a path.</p><p>The next line contains integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>).</p><p>The last line contains <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>s</i><sub class="lower-index"><i>j</i></sub></span> is the <span class="tex-span"><i>j</i></span>-th miner's height.</p></div><div class="output-specification"><p>In the single line print the minimum number of meters that you need to raise the ceiling by in some cave so that all miners could be sorted into caves and be happy about the work conditions. If it is impossible to do, print <span class="tex-span"> - 1</span>. If it is initially possible and there's no need to raise any ceiling, print <span class="tex-span">0</span>. </p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>) — the number of caves in the mine.</p><p>Then follows a line consisting of <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>h</i><sub class="lower-index">1</sub>, <i>h</i><sub class="lower-index">2</sub>, ..., <i>h</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> is the height of the ceiling in the <span class="tex-span"><i>i</i></span>-th cave.</p><p>Next <span class="tex-span"><i>n</i> - 1</span> lines contain the descriptions of transitions between the caves. Each line has the form <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are the numbers of the caves connected by a path.</p><p>The next line contains integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>).</p><p>The last line contains <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>s</i><sub class="lower-index"><i>j</i></sub></span> is the <span class="tex-span"><i>j</i></span>-th miner's height.</p>

## Output

<p>In the single line print the minimum number of meters that you need to raise the ceiling by in some cave so that all miners could be sorted into caves and be happy about the work conditions. If it is impossible to do, print <span class="tex-span"> - 1</span>. If it is initially possible and there's no need to raise any ceiling, print <span class="tex-span">0</span>. </p>





```input1
6
5 8 4 6 3 12
1 2
1 3
4 2
2 5
6 3
6
7 4 2 5 3 11

```




```input2
7
10 14 7 12 4 50 1
1 2
2 3
2 4
5 1
6 5
1 7
6
7 3 4 8 8 10

```




```input3
3
4 2 8
1 2
1 3
2
17 15

```




```output1
6

```




```output2
0

```




```output3
-1

```



## Note

<p>In the first sample test we should increase ceiling height in the first cave from <span class="tex-span">5</span> to <span class="tex-span">11</span>. After that we can distribute miners as following (first goes index of a miner, then index of a cave): <img align="middle" class="tex-formula" src="file://3dAa9trH.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>In the second sample test there is no need to do anything since it is already possible to distribute miners as following: <img align="middle" class="tex-formula" src="file://8MbOAoi3.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>In the third sample test it is impossible.</p>
